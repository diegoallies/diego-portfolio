<template>
    <div class="skills-page">
      <!-- Cover Image with Return Button -->
      <div class="cover-container">
        <router-link to="/" class="btn back-btn">
          <i class="fas fa-angle-left"></i>
          <span>Return</span>
        </router-link>
      </div>
  
      <!-- Skills Section -->
      <div class="skills-content">
        <div class="column">
          <h2 class="skills-title">Professional Skills</h2>
          <skill-bar label="JavaScript" icon="fab fa-js-square" percentage="90"></skill-bar>
          <skill-bar label="Vue.js" icon="fab fa-vuejs" percentage="80"></skill-bar>
          <skill-bar label="Angular" icon="fab fa-angular" percentage="75"></skill-bar>
          <skill-bar label="Typescript" icon="fa fa-text-width" percentage="70"></skill-bar>
          <skill-bar label="Node.js" icon="fab fa-node-js" percentage="85"></skill-bar>
          <skill-bar label="HTML5" icon="fab fa-html5" percentage="90"></skill-bar>
          
          <!-- Tech Stack skills continue here -->
        </div>
  
        <div class="column nd2">
          <!-- Place for additional professional or tech stack skills -->
          
          <skill-bar label="CSS3" icon="fab fa-css3-alt" percentage="90"></skill-bar>
          <skill-bar label="SASS" icon="fab fa-sass" percentage="80"></skill-bar>
          <skill-bar label="Git" icon="fab fa-git-alt" percentage="85"></skill-bar>
          <skill-bar label="MongoDB" icon="fab fa-mdb" percentage="70"></skill-bar>
          <skill-bar label="MySQL" icon="fas fa-database" percentage="80"></skill-bar>
          <skill-bar label="SEO" icon="fas fa-search" percentage="75"></skill-bar>
        </div>
  
        <div class="column">
          <h3 class="skills-title">Interpersonal Skills</h3>
          <skill-bar label="Problem Solving" icon="fas fa-brain" percentage="90"></skill-bar>
          <skill-bar label="Teamwork" icon="fas fa-users" percentage="85"></skill-bar>
          <skill-bar label="Public Speaking" icon="fas fa-bullhorn" percentage="75"></skill-bar>
          <skill-bar label="Adaptability" icon="fas fa-water" percentage="80"></skill-bar>
          <!-- Personal skills continue here -->
        </div>
      </div>
    </div>
  </template>
  
  <script>
  import SkillBar from '@/components/SkillBar.vue';
  
  export default {
    name: 'Skills',
    components: {
      SkillBar
    }
  };
  </script>
  
  <style scoped>

  
  .nd2 {
    margin-top: 35px !important;
  }
  .skills-page {
  height: 90vh;
  display: flex;
  flex-direction: column;
  background-color: #121212;
  color: #ffffff;

 
}

.cover-container {
  background-color: #6c7a89;
  position: relative;
  height: 55px;
  margin-bottom: 35px;
}

.btn.back-btn {
  position: absolute;
  top: 10px;
  left: 10px;
  background-color: #4c566a;
  color: #ffffff;
  padding: 0.5rem 1rem;
  border-radius: 5px;
}

.skills-content {
  display: flex;
  justify-content: space-evenly; /* Evenly distribute columns */
  align-items: flex-start; /* Align columns to the top */
  margin-inline: auto;
  max-width: 1200px; /* Max width */
  width: 100%;
}

.column {
  display: flex;
  flex-direction: column;
  align-items: flex-start; /* Align items to the left */
  width: 30%; /* Split the space by three columns */
  margin-top: -10px; /* Adjust top margin for visual alignment */
}

.skills-title {
  font-size: 1.5rem;
  margin-bottom: 1rem;
  color: #6c7a89;
}
  
  .column {
    width: 32%; /* Split the space by three columns */
  }
  
  .skills-title {
    font-size: 1.5rem;
    margin-bottom: 1rem;
    color: #6c7a89;
  }
  </style>