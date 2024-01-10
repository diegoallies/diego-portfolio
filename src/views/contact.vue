<template>
  <div class="container">
    <div class="row">
      <div class="col-sm w3-animate-left">
        <router-link to="/" class="btn btn-rabbit back-btn"><i class="fas fa-angle-left"></i><span class="back2home">Back to Home</span></router-link>
        <img src="https://i.postimg.cc/8zq0BbVB/contact.jpg" alt="me" class="contact-image">
      </div>
      <div class="col-sm w3-animate-right">
        <div class="row">
          <div class="col">
            <h1 class="contact-title">Contact</h1>
            <p class="contact-tagline">Based in Cape Town, RSA. Drop me a line here:</p>
          </div>
        </div>
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
          <button type="submit" class="btn btn-rabbit submit">Send Message</button>
        </form>
      </div>
    </div>
  </div>
  <Footer />
</template>

<script>
import Footer from '@/components/Footer.vue'

export default {
  data() {
    return {
      name: '',
      email: '',
      message: '',
    }
  },
  components: {
    Footer
  }
}
</script>

<style scoped>
.container {
  background-color: #121212; /* Dark theme background */
  color: #ffffff;
}

.contact-image {
  width: 100%;
  max-width: 400px;
  height: auto;
  margin: 2rem auto;
  display: block;
}

.contact-title {
  font-size: 2.5rem;
  font-family: "Josefin Sans", sans-serif;
}

.contact-tagline {
  font-style: italic;
  font-weight: 600;
  font-size: 1.2rem;
  line-height: 1.4;
  font-family: "Crimson", serif;
  padding-right: 2rem;
  margin-bottom: 2rem;
}

.contact-form {
  padding: 2rem;
}

.btn.btn-rabbit {
  background-color: #fff;
  color: #121212;
  border: 1px solid #fff;
  transition: all 0.4s ease-in-out;
  font-family: "Crimson", serif;
  padding: 10px 20px;
  font-size: 1rem;
  margin-top: 1rem;
  cursor: pointer;
}

.btn.btn-rabbit:hover {
  background-color: #3b3b3b;
  color: #fff;
}

.form-control {
  background-color: transparent;
  color: #fff;
  border-color: #fff;
  margin-bottom: 1rem;
}

@media only screen and (max-width: 768px) {
  /* Adjustments for mobile responsiveness */
  .contact-title,
  .contact-tagline {
    text-align: center;
  }

  .contact-form {
    padding: 1rem;
  }

  .btn.btn-rabbit {
    width: 100%;
    margin-top: 0;
  }

  .contact-image {
    margin: 1rem auto;
  }
}
</style>