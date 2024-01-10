<template>
  <div id="app" class="app-container">
    <!-- Content that takes up the main part of the screen -->
    <div class="content-container">
      <transition name="fade" mode="out-in">
        <router-view/>
      </transition>
    </div>
    <!-- Sticky Footer -->
    <Footer />
  </div>
</template>

<script>
import Footer from './components/Footer.vue';

export default {
  components: {
    Footer
  }
};
</script>

<style>
@import '~mdb-ui-kit/css/mdb.min.css';
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;500;700&display=swap');

/* Applying styles to the root element and the main #app */
html {
  height: 100%;
}

body, #app {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  background-color: #121212; /* Dark background color */
  color: #ffffff; /* Light text color */
  margin: 0;
  padding: 0;
  font-family: 'Roboto', sans-serif; /* Improved font */
}

/* Ensures that content container can expand to push the footer */
.content-container {
  flex: 1;
}

/* Animated transitions */
.fade-enter-active, .fade-leave-active {
  transition: opacity 0.5s ease;
}
.fade-enter, .fade-leave-to {
  opacity: 0;
}

/* Re-usable animations */
.w3-animate-right {
  animation: animateright 1.2s;
}
@keyframes animateright {
  from { right: -500px; opacity: 0.6; } 
  to { right: 0; opacity: 1; }
}
.w3-animate-left {
  animation: animateleft 1.2s;
}
@keyframes animateleft {
  from { left: -500px; opacity: 0.6; } 
  to { left: 0; opacity: 1; }
}

/* Media queries for responsive adjustments */
@media only screen and (max-width: 553px) {
  .w3-animate-left, .w3-animate-right {
    animation: none;
  }
}
</style>