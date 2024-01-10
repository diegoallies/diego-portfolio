<template>
  <div class="container-fluid">
      <div class="row flex-nowrap">
          <div class="col-md-6 left-column">
              <img src="https://i.postimg.cc/pd9SvZKW/wall.jpg" alt="Wallpaper" class="wallpaper-img">
          </div>
          <div class="col-md-6 right-column">
              <div class="portfolio-content">
                  <router-link to="/" class="back-btn"><i class="fas fa-angle-left"></i> Back to Home</router-link>
                  <h1 class="portfolio-title">Projects</h1>
                  <div class="projects-container">
                      <div class="project">
                          <img src="https://i.postimg.cc/J49dRJ4M/bubble-game.png" alt="Bubble Game" class="project-img">
                          <h2 class="project-title">Bubble Shooter Game</h2>
                          <p class="project-link"><a href="https://lnkd.in/dbzJEjXV" target="_blank">View on CodePen</a></p>
                      </div>
                      <div class="project">
                          <img src="https://i.postimg.cc/wBPkkYyH/otbscreenshot.png" alt="Social Media Platform" class="project-img">
                          <h2 class="project-title">Social Media Platform</h2>
                          <p class="project-description">A social media platform I'm currently developing for a client.</p>
                      </div>
                  </div>
              </div>
          </div>
      </div>
  </div>
  
  <Footer />
  </template>
  
  <script>
  import Footer from '@/components/Footer.vue'
  
  export default {
      components: {
          Footer
      }
  }
  </script>
  
  <style scoped>
  
  .container-fluid {
      padding: 0;
      overflow: hidden;
  }
  
  .left-column {
      position: relative;
  }
  
  .wallpaper-img {
      width: 100%;
      height: 100vh;
      object-fit: cover;
  }
  
  .right-column {
      padding: 4vh 4vw;
      background-color: #121212; /* Dark theme background */
      color: #ffffff;
      display: flex;
      flex-direction: column;
  }
  
  .portfolio-content {
      max-width: 600px;
      margin: auto;
  }
  
  .back-btn {
      font-size: 1.2rem;
      margin-bottom: 2rem;
      color: #ffffff;
      text-decoration: none;
  }
  
  .portfolio-title {
      font-size: 2.5rem;
      font-family: "Josefin Sans", sans-serif;
      margin-bottom: 1rem;
  }
  
  .projects-container {
      margin-top: 1rem;
  }
  
  .project {
      margin-bottom: 2rem;
      text-align: center;
  }
  
  .project-img {
      max-width: 100%;
      margin-bottom: 1rem;
      border-radius: 5px;
  }
  
  .project-title {
      font-size: 1.5rem;
      font-family: "Crimson", serif;
      margin-bottom: 0.5rem;
  }
  
  .project-link a, .project-description {
      font-size: 1rem;
      color: #aaa;
      text-decoration: none;
      font-style: italic;
  }
  
  .project-link a:hover {
      color: #fff;
      text-decoration: underline;
  }
  
  @media only screen and (max-width: 768px) {
      .left-column, .right-column {
          flex: 0 0 100%;
          max-width: 100%;
      }
      
      .wallpaper-img {
          height: auto;
      }
  
      .portfolio-content {
          padding: 3vh 3vw;
      }
  }
  </style>