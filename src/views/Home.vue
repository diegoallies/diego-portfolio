<template>
  <div class="home" id="index">
    <!-- Cover Image Container -->
    <div class="cover-container">
      <!-- Profile Image Container -->
      <div class="profile-container">
        <div class="tech-icons tech-icons-left">
          <i class="fab fa-vuejs"></i> <!-- Vue.js -->
          <i class="fab fa-js"></i> <!-- JavaScript -->
          <i class="fab fa-sass"></i> <!-- SCSS -->
          <i class="fab fa-angular"></i> <!-- Angular -->
          <i class="fab fa-react"></i> <!-- React -->
          <i class="fab fa-css3"></i> <!-- CSS3 -->
        </div>
        <img src="https://i.postimg.cc/rsJjxhBL/diego.jpg" alt="Diego Allies" class="profile-image">
        <div class="tech-icons tech-icons-right">
          <i class="fas fa-database"></i> <!-- MySQL -->
          <i class="fab fa-node-js"></i> <!-- Node.js -->
          <i class="fab fa-node"></i> <!-- Placeholder for Express.js -->
          <i class="fab fa-reacteurope"></i> <!-- Placeholder for Next.js (Creative use) -->
          <i class="fas fa-cloud"></i>
          <i class="fab fa-mdb"></i> <!-- MongoDB -->
        </div>
      </div>
    </div>
    <!-- Content Container -->
    <div class="contentContainer">
      <h1 class="headline">Diego Allies - Software Engineer</h1>
      <p class="intro">Crafting robust solutions with a blend of modern technologies and a passion for continuous learning in software engineering.</p>
      <div class="navigation">
        <router-link to="/about" class="btn btn-custom">About</router-link>
        <router-link to="/skills" class="btn btn-custom">Skills</router-link>
        <router-link to="/projects" class="btn btn-custom">Projects</router-link>
        <router-link to="/contact" class="btn btn-custom">Contact</router-link>
      </div>
      <div class="social-links">
        <a href="mailto:diegoallies27@gmail.com" class="social-icon"><i class="fab fa-google"></i></a>
        <a href="https://www.linkedin.com/in/diego-allies/" class="social-icon"><i class="fab fa-linkedin-in"></i></a>
        <a href="https://github.com/diegoallies" class="social-icon"><i class="fab fa-github"></i></a>
        <a href="https://wa.me/2779354808" class="social-icon"><i class="fab fa-whatsapp"></i></a>
      </div>
    </div>
  </div>
</template>


<script>
export default {
  name: 'Home'
};
</script>

<style scoped>
.home {
  display: flex;
  flex-direction: column;
  align-items: center;
  background-color: #121212;
  color: #ffffff;
  text-align: center;
  padding: 0;
  margin: 0;
}

.cover-container {
  position: relative;
  width: 100%;
  height: 200px;
  background-color: #6c7a89;
  margin-bottom: 60px;
}

.cover-image {
  width: 100%;
  height: 100%;
  object-fit: cover;
}


.tech-icons {
  display: flex;
  justify-content: center;
  align-items: center;
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
}

.tech-icons-left {
  left: calc(50% - 230px - 120px); /* Adjust based on the desired space between icons and image */
  margin-top: 40px;
}

.tech-icons-right {
  right: calc(50% - 250px - 120px); /* Adjust based on the desired space between icons and image */
  margin-top: 40px;
}

.tech-icons i {
  color: #6c7a89; /* Matching the theme color */
  margin: 0 5px;
  font-size: 24px; /* Icon size, adjust as needed */
  transition: color 0.3s ease;
}

.tech-icons i:hover {
  color: #ffffff;
}
.profile-container {
  position: absolute;
  left: 50%;
  bottom: -125px;
  transform: translateX(-50%);
  border: 5px solid #121212;
  border-radius: 50%;
  background-color: #fff;
  padding: 5px;
}

.profile-image {
  width: 250px;
  height: 250px;
  border-radius: 50%;
  object-fit: cover;
}

.headline {
  margin-top: 90px;
  font-size: 2.5rem;
}

.intro {
  font-size: 1.25rem;
  margin: 20px 0;
}

.navigation {
  margin-bottom: 20px;
}

.btn.btn-custom {
  background-color: #6c7a89;
  color: #121212;
  margin: 10px;
  padding: 10px 20px;
}

.social-links {
  margin-bottom: 50px;
}

.social-icon {
  color: #ffffff;
  font-size: 1.5rem;
  margin: 0 10px;
}

.social-icon:hover {
  color: #bbbbbb;
}

@media (max-width: 600px) {
  .headline {
    font-size: 2rem;
  }
  .profile-container {
    bottom: -50px;
  }
  .profile-image {
    width: 100px;
    height: 100px;
  }
}
</style>