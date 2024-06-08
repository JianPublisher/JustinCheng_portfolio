<template>
  <nav-bar></nav-bar>
  <div class="content">
    <img src="@/assets/profile.jpg" alt="Profile Picture" class="profile-picture" />
    <h1>Justin Cheng</h1>
    <h2>Software Developer</h2>
    <p>Welcome to my portfolio page! I'm a software engineer with machine learning experience. Feel free to explore my projects and don't hesitate to reach out. I'd love to connect with you!</p>
    
    <div class="button-container">
      <a href="https://www.linkedin.com/in/jchengyj" target="_blank" class="nav-button">LinkedIn</a>
      <a href="https://github.com/JianPublisher" target="_blank" class="nav-button">GitHub</a>
    </div>

    <div class="section" id="projects">
    <h2>Projects</h2>
    <div class="projects-container">
      <div class="project-card">
        <a href="https://github.com/JianPublisher/Exam-Proctor-Website" target="_blank">
          <img src="@/assets/photo1.png" alt="Project 1" class="project-image" />
        </a>
      </div>
      <div class="project-card">
        <a href="https://github.com/JianPublisher/Donation-Website" target="_blank" class="project-link">
          <img src="@/assets/photo2.png" alt="Project 2" class="project-image" />
        </a>
      </div>
            <div class="project-card">
        <a href="https://github.com/JianPublisher/Brick-Game-" target="_blank" class="project-link">
          <img src="@/assets/photo3.png" alt="Project 2" class="project-image" />
        </a>
      </div>
      <div class="project-card">
        <a href="https://github.com/JianPublisher/Car-Game" target="_blank" class="project-link">
          <img src="@/assets/photo4.png" alt="Project 2" class="project-image" />
        </a>
      </div>
      <div class="project-card">
        <a href="https://dl.acm.org/doi/10.1145/3477314.3507200" target="_blank" class="project-link">
          <p>( ͡° ͜ʖ ͡° )</p>
        </a>
      </div>
    </div>
  </div>
  </div>
  

  <div class="section" id="contact">
    <h2>Contact Me</h2>
    <form class="contact-form" action="https://formspree.io/f/meqybdww" method="POST">
      <label for="name">Name</label>
      <input type="text" id="name" name="name" required />
      
      <label for="email">Email</label>
      <input type="email" id="email" name="email" required />
      
      <label for="message">Message</label>
      <textarea id="message" name="message" rows="5" required></textarea>
      
      <button type="submit">Send</button>
    </form>
  </div>
</template>

<script>
import NavBar from './NavBar.vue';
export default {
  name: 'MainPage',
  components: {
    NavBar
  },
};
</script>

<style scoped src="@/assets/MainPage.css"></style>
