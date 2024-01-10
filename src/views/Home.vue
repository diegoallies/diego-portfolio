<template>
  <div class="home" id="index">
    <!-- Cover Image Container -->
    <div class="cover-container">
      <img src="https://media.licdn.com/dms/image/D5616AQHiwSdHXe9xfQ/profile-displaybackgroundimage-shrink_350_1400/0/1695365316064?e=1710374400&v=beta&t=lCyaBIbzRrJff_WqBRAcUs3gQvWSJDJ_Y7qoS2jWXNg" alt="Cover" class="cover-image">
      <!-- Profile Image Container -->
      <div class="profile-container">
        <img src="https://i.postimg.cc/rsJjxhBL/diego.jpg" alt="Diego Allies" class="profile-image">
      </div>
    </div>
    <!-- Content Container -->
    <div class="contentContainer">
      <h1 class="headline">I am Diego Allies</h1>
      <p class="intro">I am a Junior Web developer able to build a Web presence from the ground up - from concept, navigation, layout and programming to UX and SEO...</p>
      <div class="navigation">
        <router-link to="/about" class="nav-btn">About</router-link>
        <router-link to="/skills" class="nav-btn">Skills</router-link>
        <router-link to="/projects" class="nav-btn">Projects</router-link>
        <router-link to="/contact" class="nav-btn">Contact</router-link>
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
import Footer from '@/components/Footer.vue';

export default {
  name: 'Home',
  components: {
    Footer
  }
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
  padding-bottom: 3rem; /* space for the footer */
}

.cover-container {
  position: relative;
  width: 100%;
  height: 200px; /* Set the height for your cover image */
  background-color: #6c7a89; /* placeholder in case image fails to load */
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
  display: block;
  width: 250px;
  height: 250px;
  border-radius: 50%;
  object-fit: cover;
}

.headline {
  margin: 100px 0 20px; /* Adjust space for profile image */
  font-size: 2.5rem;
}

.intro, .navigation {
  margin-bottom: 1rem;
}

.nav-btn {
  display: inline-block;
  margin: 0.5rem;
  padding: 0.5rem 1rem;
  color: #ffffff;
  background-color: #007bff; /* Bootstrap primary blue */
  text-decoration: none;
  border: none;
  border-radius: 2px;
  font-size: 1rem;
  transition: all 0.2s ease-in-out;
}

.nav-btn:hover {
  background-color: #0056b3; /* Darken on hover */
}

.social-icon {
  font-size: 1.5rem;
  margin: 0 0.5rem;
  color: #ffffff;
  text-decoration: none;
  transition: all 0.2s ease-in-out;
}

.social-icon:hover {
  opacity: 0.8;
}

@media (max-width: 600px) {
  .headline {
    font-size: 2rem;
  }
  .profile-container {
    bottom: -50px; /* Adjust profile position for smaller screens */
  }
  .profile-image {
    width: 100px;
    height: 100px;
  }
}
</style>