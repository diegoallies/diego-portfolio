<template>
  <div class="container">
    <div class="row">
      <div class="col-sm w3-animate-left">
        <router-link to="/" class="btn btn-rabbit back-btn"><i class="fas fa-angle-left"></i><span class="back2home">Back to Home</span></router-link>
        <img src="https://i.postimg.cc/hjBt49rF/meee.jpg" alt="Diego Allies" class="abt-image">
      </div>
      <div class="col-sm w3-animate-right">
        <div class="about-content">
          <h1 class="abttt">About</h1>
          <h2 class="subt">Hi, I am Diego Allies - Fullstack Web Developer</h2>
          <p class="main-txt">I am a competent Software Engineer, capable of building a diverse range of software systems from conception to launch. Proficient in writing well-structured, efficient, and testable code that adheres to current industry-best practices.</p>
          <p class="main-txt">Known for my rapid learning ability and strong work ethic, I'm a team player who excels in various scripting languages. With an extensive skill set and a deep understanding of the software development life cycle, I aim to deliver top-tier software solutions.</p>
          <p class="main-txt">Driven by innovation, commitment to excellence, and a passion for continuous learning, I am an invaluable addition to any progressive software team.</p>
        </div>
      </div>
    </div>
  </div>
  <Footer />
  </template>
  
  <script>
  import * as mdb from 'mdb-ui-kit';
  import { input } from 'mdb-ui-kit';
  import Footer from '@/components/Footer.vue';
  
  export default {
    components: {
      Footer
    }
  }
  </script>
  
  <style scoped>
  .container {
    background-color: #121212; /* Dark theme background */
    color: #ffffff;
    max-width: 100%;
  }
  
  .abt-image {
    width: 100%;
    max-width: 400px;
    height: auto;
    margin: 2rem auto;
    display: block;
  }
  
  .back-btn {
    margin-top: 15%;
    color: #ffffff;
    border-color: #ffffff; /* Colors adjusted for dark theme */
  }
  
  .back2home {
    font-family: "Josefin Sans", sans-serif;
  }
  
  .about-content {
    padding: 2rem;
  }
  
  .abttt {
    font-size: 2.5rem;
    font-family: "Josefin Sans", sans-serif;
    margin-bottom: 1rem;
  }
  
  .subt {
    font-style: italic;
    font-weight: 600;
    font-size: 1.75rem;
    line-height: 1.4;
    font-family: "Crimson", serif;
    margin-bottom: 2rem;
  }
  
  .main-txt {
    font-size: 1rem;
    margin-bottom: 1rem;
    line-height: 1.6;
  }
  
  .btn {
    padding: 0.375rem 1.5rem;
  }
  
  @media only screen and (max-width: 768px) {
    .back-btn {
      margin-top: 1rem;
    }
  
    .abttt,
    .subt {
      text-align: center;
      margin-left: 0;
      margin-top: 1rem;
    }
  
    .main-txt {
      text-align: justify;
      margin-left: 0;
    }
  }
  </style>