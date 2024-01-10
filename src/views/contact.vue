<template>
  <div class="contact-page">
    <!-- Return Button -->
    <div class="cover-container">
      <router-link to="/" class="btn back-btn">
        <i class="fas fa-angle-left"></i>
        <span>Return</span>
      </router-link>
    </div>

    <!-- Contact Form Section -->
    <div class="contact-content">
      <h1 class="contact-title">Contact</h1>
      <p class="contact-tagline">Based in Cape Town, RSA. Drop me a line here:</p>
      
      <form class="contact-form" action="https://formspree.io/f/xnqwyraz" method="POST">
        <div class="form-group">
          <input type="text" class="form-control" id="exampleInputName" placeholder="Name" name="Name" v-model="name">
        </div>
        <div class="form-group">
          <input type="email" class="form-control" id="exampleInputEmail1" placeholder="Email" name="_replyto" v-model="email">
        </div>
        <div class="form-group">
          <textarea class="form-control" rows="5" placeholder="Message" name="Message" v-model="message"></textarea>
        </div>
        <button type="submit" class="btn btn-custom submit">Send Message</button>
      </form>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      name: '',
      email: '',
      message: '',
    }
  },
};
</script>

<style scoped>
.contact-page {
  display: flex;
  flex-direction: column;
  align-items: center;
  background-color: #121212;
  color: #ffffff;
  text-align: center;
  padding: 0;
  height: 90vh;
  min-height: calc(100vh - 200px); /* Account for 200px footer */
  padding-bottom: 200px; /* Footer space */
}

.cover-container {
  background-color: #6c7a89;
  width: 100%;
  padding-top: 70px;
  position: relative;
  margin-bottom: 60px;
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

.contact-content {
  width: 80%;
  max-width: 600px;
}

.contact-title {
  font-size: 2.5rem;
  color: #6c7a89;
  margin-bottom: 1rem;
}

.contact-tagline {
  font-size: 1.25rem;
  margin-bottom: 2rem;
}

.contact-form {
  text-align: left;
}

.form-group {
  margin-bottom: 1rem;
}

.form-control {
  width: 100%;
  background-color: transparent;
  color: #fff;
  border: 1px solid #fff;
  border-radius: 5px;
  padding: 0.5rem;
  margin-bottom: 1rem;
}

.btn.btn-custom {
  background-color: #6c7a89;
  color: #121212;
  margin: 10px;
  padding: 10px 20px;
}

.submit {
  cursor: pointer;
  width: 100%;
  padding: 10px;
  font-size: 1rem;
  border: none;
  transition: all 0.2s ease-in-out;
}

.submit:hover {
  background-color: #4c566a;
  color: #ffffff;
}
</style>