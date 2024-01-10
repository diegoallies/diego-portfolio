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
      <div class="skills-grid">
        <!-- Each SkillBar component represents a skill with a labelled bar to the set percentage -->
        <skill-bar label="JavaScript" icon="fab fa-js-square" percentage="90"></skill-bar>
        <skill-bar label="Vue.js" icon="fab fa-vuejs" percentage="80"></skill-bar>
        <skill-bar label="Angular" icon="fab fa-angular" percentage="75"></skill-bar>
        <skill-bar label="SASS" icon="fab fa-sass" percentage="70"></skill-bar>
        <skill-bar label="Node.js" icon="fab fa-node-js" percentage="85"></skill-bar>
        <skill-bar label="HTML 5" icon="fab fa-html5" percentage="90"></skill-bar>
        <skill-bar label="CSS 3" icon="fab fa-css3-alt" percentage="90"></skill-bar>
        <!-- Add other skill bars here -->
        <!-- ... -->
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
  .skills-page {
    display: flex;
    flex-direction: column;
    align-items: center;
    background-color: #121212;
    color: #ffffff;
    text-align: center;
    padding-bottom: 200px; /* Adjust for footer */
    height: 100vh; /* Adjust the height of this component to prevent scrolling */
    overflow: hidden; /* Hide overflow */
  }
  
  .cover-container {
    background-color: #6c7a89;
    height: 200px;
    position: relative;
    width: 100%;
  }
  
  .btn.back-btn {
    position: absolute;
    top: 1rem;
    left: 1rem;
    background-color: #4c566a;
    color: #ffffff;
    border: none;
    padding: 0.5rem 1rem;
    border-radius: 5px;
    text-decoration: none;
  }
  
  .skills-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
    gap: 1rem;
    width: 80%;
    padding-top: 1rem;
  }
  
  /* Style for .cover-container, .btn.back-btn, as well as additional global styles are unchanged */
  
  </style>