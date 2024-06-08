<template>
  <nav class="navbar">
    <div class="logo">Justin Cheng</div>
    <div class="nav-links">
      <a href="#projects" class="nav-button">View Projects</a>
      <a href="#contact" class="nav-button">Contact Me</a>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'NavBar'
}
</script>

<style scoped>
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem 2rem;
  background-color: rgba(255, 255, 255, 0.8); /* Semi-transparent background */
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  backdrop-filter: blur(10px); /* Blur effect */
  position: sticky;
  top: 0;
  z-index: 1000;
}

.logo {
  font-size: 2rem;
  font-weight: 700;
  color: #0077b5;
  text-transform: uppercase;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  letter-spacing: 2px;
  transition: color 0.3s, transform 0.3s;
}

.logo:hover {
  color: #005582;
  transform: scale(1.05);
}

.nav-links {
  display: flex;
  gap: 1.5rem;
}

.nav-button {
  background-color: #fff;
  color: #333;
  border: 2px solid #0077b5;
  padding: 0.5rem 1.5rem;
  text-decoration: none;
  border-radius: 25px;
  transition: background-color 0.3s, color 0.3s, transform 0.3s, box-shadow 0.3s;
  font-weight: 600;
}

.nav-button:hover {
  background-color: #0077b5;
  color: #fff;
  transform: translateY(-2px);
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
}

.nav-button:nth-child(2):hover {
  background-color: #333;
  color: #fff;
  transform: translateY(-2px);
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
}

@media (max-width: 768px) {
  .navbar {
    flex-direction: column;
    align-items: flex-start;
    padding: 1rem;
  }
  
  .nav-links {
    flex-direction: column;
    gap: 0.5rem;
    width: 100%;
  }
  
  .nav-button {
    width: 100%;
    text-align: center;
    padding: 0.75rem 0;
  }
}
</style>
