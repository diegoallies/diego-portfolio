<template>
  <div class="about-page">
    <!-- Cover Image with Back Button -->
    <div class="cover-container">
      <div class="cover-image">
        <router-link to="/" class="btn back-btn">
          <i class="fas fa-angle-left"></i>
          <span>Return</span>
        </router-link>
      </div>
    </div>

    <!-- Bio, Work Experience, and Contact Section -->
    <div class="main-content">
      <!-- Work Experience Section -->
      <div class="timeline-section">
        <h4>Work Experience</h4>
        <div class="timeline">
          <div class="timeline-item">
            <div class="timeline-dot"></div>
            <p>Software Developer at Arealytics SA</p>
            <p>21 Feb 2023 - Present</p>
          </div>
          <div class="timeline-item">
            <div class="timeline-dot"></div>
            <p>Frontend Software Developer at Cimso BS</p>
            <p>12 July 2022 - 30 October 2022</p>
          </div>
          <div class="timeline-item">
            <div class="timeline-dot"></div>
            <p>Fullstack Website Developer at LC Studios</p>
            <p>11 April 2022 - 12 July 2022</p>
          </div>
        </div>
      </div>

      

      <!-- Bio and Profile Section -->
      <div class="profile-bio-section">
        <h2>DIEGO ALLIES</h2>
        <h3>SOFTWARE ENGINEER</h3>
        <div class="biography">
          <p>As a Software Engineer with two years' experience, I bring a full-stack perspective to web development. My skill set spans SQL databases, API integration, and crafting responsive interfaces across various JavaScript frameworks. With strong foundations in coding, I'm well-prepared to contribute to your projects.</p>
        </div>
      </div>

      <!-- Separator Line -->
      <div class="separator"></div>
      <div class="separator2"></div>

      <!-- Contact Information Section -->
      <div class="contact-information">
        <h4>Contact</h4>
        <div class="contact-item">
          <i class="fas fa-phone-alt contact-icon"></i>
          <p class="contact-text">0679354808</p>
        </div>
        <div class="contact-item">
          <i class="fas fa-envelope contact-icon"></i>
          <p class="contact-text">diegoallies27@gmail.com</p>
        </div>
        <div class="contact-item">
          <i class="fas fa-home contact-icon"></i>
          <p class="contact-text">Cape Town , South Africa</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'About',
};
</script>

<style scoped>
.about-page {
  display: flex;
  flex-direction: column;
  height: 80vh;
  background-color: #121212;
  color: #ffffff;
  font-family: 'Arial', sans-serif;
  padding-bottom: 200px; /* Space for footer */
}

.cover-container {
  position: relative;
}

.cover-image {
  background-image: url('https://i.postimg.cc/kGg1JcPj/coverimg.jpg');
  background-size: cover;
  background-position: center;
  height: 25vh;
  margin-bottom: 50px;
}

.btn.back-btn {
  position: absolute;
  top: 20px;
  left: 20px;
  background-color: rgba(76, 86, 106, 0.7);
  border: none;
  color: #ffffff;
  padding: 10px 15px;
  border-radius: 5px;
  text-decoration: none;
  font-size: 14px;
}

.main-content {
  display: flex;
  justify-content: space-around;
  align-items: flex-start;
  padding: 0 2vw;
  height: 55vh;
}

.timeline-section {
  flex-basis: 30%;
  padding-right: 2vw;
}

.timeline {
  position: relative;
  border-left: 2px solid #6c7a89;
  padding-left: 12px;
}

.timeline-dot {
  position: absolute;
  left: -20px;
  top: 5px;
  width: 15px;
  height: 15px;
  background-color: #6c7a89;
  border-radius: 50%;
  z-index: 1;
}

.timeline-item {
  position: relative;
  padding-bottom: 20px;
}

.timeline-content {
  position: relative;
  padding-left: 10px;
}
.separator {
  width: 2px; /* Width of the separator line */
  background-color: #6c7a89; /* Color of the separator line */
  height: 450px; /* Adjust the height as needed */
  align-self: center; /* Center the line if the parent is a flex container */
  margin-top: -100px;
  margin-left: 0;
  margin-right: 0;
}
.separator2 {
  width: 2px; /* Width of the separator line */
  background-color: #6c7a89; /* Color of the separator line */
  height: 250px; /* Adjust the height as needed */
  align-self: center; /* Center the line if the parent is a flex container */
  margin-top: -125px;
  margin-left: -30px;
  margin-right: 0;
}

.profile-bio-section {
  flex-basis: 40%;
  text-align: right;
  max-width: 400px; /* Adjust width as needed */
}

.biography {
  background-color: rgba(255, 255, 255, 0.1);
  padding: 10px;
  margin-top: 10px;
  text-align: justify;
  border: 1px solid #6c7a89;
}

.contact-information {
  color: #ffffff;
}

.contact-information h4 {
  margin-bottom: 15px;
  color: #6c7a89;
  font-weight: 600;
}

.contact-item {
  display: flex;
  align-items: center;
  margin-bottom: 10px;
}

.contact-icon {
  margin-right: 10px;
  color: #6c7a89;
  width: 20px; /* Adjust the width as desired */
  text-align: center;
}

.contact-text {
  margin: 0;
  font-size: 0.9rem; /* Adjust font-size as needed */
}

h2, h3, h4 {
  color: #6c7a89;
}
</style>