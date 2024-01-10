<template>
  <div class="home" id="index">
    <!-- Cover Image Container -->
    <div class="cover-container">
      <!-- <img src="https://media.licdn.com/dms/image/D5616AQHiwSdHXe9xfQ/profile-displaybackgroundimage-shrink_350_1400/0/1695365316064?e=1710374400&v=beta&t=lCyaBIbzRrJff_WqBRAcUs3gQvWSJDJ_Y7qoS2jWXNg" alt="Cover" class="cover-image"> -->
      <!-- Profile Image Container -->
      <div class="profile-container">
        <img src="https://i.postimg.cc/rsJjxhBL/diego.jpg" alt="Diego Allies" class="profile-image">
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