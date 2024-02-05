<template>
  <div class="about-page">
    <div class="cover-container">
      <div class="cover-image">
        <router-link to="/" class="btn back-btn">
          <i class="fas fa-angle-left"></i>
          <span>Return</span>
        </router-link>
      </div>
    </div>

    <div class="main-content">
      <div class="timeline-section">
        <h4>Work Experience</h4>
        <div class="timeline">
          <div class="timeline-item">
            <div class="timeline-dot"></div>
            <p>Software Developer at Databalk</p>
            <p>Jan 2024 - Present</p>
          </div>
          <div class="timeline-item">
            <div class="timeline-dot"></div>
            <p>Software Developer at Arealytics SA</p>
            <p>Feb 2023 - Jan 2024</p>
          </div>
          <div class="timeline-item">
            <div class="timeline-dot"></div>
            <p>Frontend Software Developer at Cimso BS</p>
            <p>July 2022 - Oct 2022</p>
          </div>
          <div class="timeline-item">
            <div class="timeline-dot"></div>
            <p>Fullstack Website Developer at LC Studios</p>
            <p>April 2022 - July 2022</p>
          </div>
        </div>
      </div>

      <div class="profile-bio-section">
        <h2>DIEGO ALLIES</h2>
        <h3>SOFTWARE ENGINEER</h3>
        <div class="biography">
          <p>As a Software Engineer with two years' experience, I bring a full-stack perspective to web development. My skill set spans SQL databases, API integration, and crafting responsive interfaces across various JavaScript frameworks. With strong foundations in coding, I'm well-prepared to contribute to your projects.</p>
        </div>
      </div>

      <div class="separator"></div>
      <div class="separator2"></div>

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
          <p class="contact-text">Cape Town, South Africa</p>
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
  min-height: 100vh;
  background-color: #121212;
  color: #ffffff;
  font-family: 'Arial', sans-serif;
  padding-bottom: 20px; /* Space adjusted for mobile view */
}

.cover-container {
  position: relative;
}

.cover-image {
  background-image: url('https://i.postimg.cc/kGg1JcPj/coverimg.jpg');
  background-size: cover;
  background-position: center;
  height: 25vh;
  margin-bottom: 20px; /* Space adjusted for mobile view */
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
  flex-direction: column; /* Changed for mobile-first */
  align-items: center; /* Align items for mobile view */
  justify-content: space-around;
  padding: 0 5%; /* Padding adjusted for mobile view */
}

.timeline-section,
.profile-bio-section,
.contact-information {
  width: 100%; /* Full width for mobile-first */
  max-width: 600px; /* Ensuring content doesn't stretch too far on larger screens */
  margin-bottom: 20px; /* Space between sections */
}

.timeline {
  border-left: 2px solid #6c7a89;
  padding-left: 12px;
}

.timeline-dot {
  position: absolute;
  left: -8px; /* Adjusted for better center alignment */
  top: 5px;
  width: 15px;
  height: 15px;
  background-color: #6c7a89;
  border-radius: 50%;
}

.timeline-item p {
  margin: 5px 0; /* Adjusted margin for better readability */
}

.separator, .separator2 {
  display: none; /* Hidden in mobile view for simplicity */
}

.biography {
  background-color: rgba(255, 255, 255, 0.1);
  padding: 10px;
  margin-top: 10px;
  border: 1px solid #6c7a89;
}

.contact-item {
  display: flex;
  align-items: center;
  margin-bottom: 10px;
}

.contact-icon {
  margin-right: 10px;
  color: #6c7a89;
}

.contact-text, h2, h3, h4 {
  color: #6c7a89;
}

@media (min-width: 768px) { /* Adjustments for tablets and up */
  .main-content {
    flex-direction: row; /* Back to row for wider screens */
    align-items: flex-start;
    padding: 0 2vw;
  }

  .timeline-section, .profile-bio-section, .contact-information {
    flex-basis: 30%; /* Adjust flex-basis for distribution */
  }

  .separator, .separator2 {
    display: block; /* Show separators on bigger screens */
    width: 2px;
    background-color: #6c7a89;
    height: 250px; /* Adjusted height */
    align-self: center;
    margin: 0 20px; /* Add some space around separators */
  }

  .separator2 {
    height: 150px; /* Shorter for design purposes */
    margin-left: -30px; /* Adjusted positioning */
  }
}
</style>