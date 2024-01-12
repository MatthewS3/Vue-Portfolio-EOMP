<template>
  <div class="loader">
    <div class="progress-bar"></div>
  </div>
  <div class="contact">
    <h1>Contact Me:</h1>
  </div>
  <section class="contact-page-sec">
    <div class="container">
      <div class="row">
        <div class="col-md-4">
          <div class="contact-info">
            <div class="contact-info-item">
              <div class="contact-info-icon">
                <i class="fas fa-map-marked"></i>
              </div>
              <div class="contact-info-text">
                <h2>location</h2>
                <span> 89 Gladiola Road, Lavender Hill </span>
                <span>Cape Town , South Africa</span>
              </div>
            </div>
          </div>
        </div>
        <div class="col-md-4">
          <div class="contact-info">
            <div class="contact-info-item">
              <div class="contact-info-icon">
                <i class="fas fa-envelope"></i>
              </div>
              <div class="contact-info-text">
                <h2>E-mail & Cell</h2>
                <span>mtthwswain@gmail.com</span>
                <span>(079) 318 2409 </span>
              </div>
            </div>
          </div>
        </div>
        <div class="col-md-4">
          <div class="contact-info">
            <div class="contact-info-item">
              <div class="contact-info-icon">
                <i class="fas fa-clock"></i>
              </div>
              <div class="contact-info-text">
                <h2>Availibilty</h2>
                <span>Mon - Fri 9:00 am - 5.00 pm</span>
                <span>Sat & Sun 10.00 pm - 2.00 pm</span>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="row">
        <div class="col-md-8">
          <div class="contact-page-form">
            <form @submit.prevent="submitForm" method="post" action="https://formspree.io/f/xleqdjjr">
              <div class="row">
                <div class="col-md-6 col-sm-6 col-xs-12">
                  <div class="single-input-field">
                    <input type="text" placeholder="Your Name" name="name" v-model="formData.name"  required />
                  </div>
                </div>
                <div class="col-md-6 col-sm-6 col-xs-12">
                  <div class="single-input-field">
                    <input type="email" placeholder="E-mail" name="email" v-model="formData.email" required />
                  </div>
                </div>
                <div class="col-md-6 col-sm-6 col-xs-12">
                  <div class="single-input-field">
                    <input type="text" placeholder="Phone Number" name="phone" v-model="formData.message" required />
                  </div>
                </div>
                <div class="col-md-12 message-input">
                  <div class="single-input-field">
                    <textarea placeholder="Write Your Message" name="message"></textarea>
                  </div>
                </div>
                <div class="single-input-fieldsbtn">
                  <button type="submit">Send</button>
                </div>
              </div>
            </form>
          </div>
        </div>
        <div class="col-md-4">
          <div class="contact-page-map">
            <iframe
              src="https://www.google.com/maps/embed/v1/place?q=Lavender+Hill,+Cape+Town,+South+Africa&key=AIzaSyBFw0Qbyq9zTFTd-tUY6dZWTgaQzuU17R8"
              width="310"
              height="400"
              frameborder="0"
              style="border: 0"
              allowfullscreen
            ></iframe>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
// @ is an alias to /src

import axios from 'axios'
export default {
  components: {
    
  },
  data() {
  return {
    formData: {
      name: '',
      email: '',
      message: '',
      phone:''
    }
  }
},
methods: {
  async submitForm() {
    try {
      // You can add form validation logic here if needed
      console.log('Form submitted with data:', this.formData);
      // If you want to send an AJAX request, you can use libraries like Axios
      // Example using Axios:
      await axios.post('https://formspree.io/f/xleqdjjr', this.formData);
      // Reset the form after submission
      this.formData = {
        name: '',
        email: '',
        message: ''
      };
    } catch (error) {
      console.error('Error submitting form:', error);
    }
  }
}
}
</script>

<style>

.loader {
    width: 100%;
    height: 100%;
    background-color: #333;
    position: absolute;
    top: 0;
    left: 0;
    -webkit-animation: loader 0.5s 5s ease forwards;
    animation: loader 1.5s 5s ease-in forwards;
    z-index: 99;
}

.progress-bar {
    width: 200px;
    height: 2px;
    background-color: black;
    position: relative;
    top: calc(50% - 1px);
    left: calc(50% - 100px);
}

.progress-bar:before {
    content: "";
    display: block;
    width: 0px;
    height: 4px;
    position: absolute;
    top: -1px;
    border-left: 0px solid Gold;
    -webkit-animation: progress 6s ease-in-out forwards;
    animation: progress 5s ease-in-out forwards;
}

@-webkit-keyframes loader {
    to {left: -100%;}
}

@keyframes loader {
    to {left: -100%;}
}

@-webkit-keyframes progress {
    to {border-left: 200px solid Gold;}
}

@keyframes progress {
    to {border-left: 200px solid Gold;}
}

/* page loader */
.contact-info {
  display: inline-block;
  width: 100%;
  text-align: center;
  margin-bottom: 10px;
}
.contact-info-icon {
  margin-bottom: 15px;
}
.contact-info-item {
  background: gold;
  border-radius: 50px;
  padding: 103px 0px;
}
.contact-page-sec .contact-page-form h2 {
  color: #071c34;
  text-transform: capitalize;
  font-size: 22px;
  font-weight: 700;
}
.contact-page-form .col-md-6.col-sm-6.col-xs-12 {
  padding-left: 0;
}
.contact-page-form.contact-form input {
  margin-bottom: 5px;
}
.contact-page-form.contact-form textarea {
  height: 110px;
}
.contact-page-form.contact-form input[type="submit"] {
  background: black;
  width: 150px;
  border-color: blsck;
}
.contact-info-icon i {
  font-size: 48px;
  color: #fda40b;
}
.contact-info-text p {
  margin-bottom: 0px;
}
.contact-info-text h2 {
  color: black;
  font-size: 22px;
  text-transform: capitalize;
  font-weight: 600;
  margin-bottom: 10px;
}
.contact-info-text span {
  color: #222;
  font-size: 16px;
  display: inline-block;
  width: 100%;
}

.contact-page-form input {
  background: #ddd none repeat scroll 0 0;
  border: 2px solid #111;
  margin-bottom: 20px;
  padding: 12px 16px;
  width: 100%;
  border-radius: 40px;
}

.contact-page-form .message-input {
  display: inline-block;
  width: 100%;
  padding-left: 0;
}
.single-input-field textarea {
  background: #ddd none repeat scroll 0 0;
  border: 2px solid #000;
  width: 100%;
  height: 120px;
  padding: 12px 16px;
  border-radius: 20px;
}
.single-input-fieldsbtn button[type="submit"] {
  background: #111 none repeat scroll 0 0;
  color: gold;
  display: inline-block;
  font-weight: 600;
  padding: 10px 0;
  text-transform: capitalize;
  width: 150px;
  margin-top: 20px;
  font-size: 16px;
}
.single-input-fieldsbtn button[type="submit"]:hover {
  background: gold;
  color: black;
  transition: all 0.7s ease-in-out 0s;
  border-color: #071c34;
  cursor: pointer;
}
.single-input-field h4 {
  color: #464646;
  text-transform: capitalize;
  font-size: 14px;
}
.contact-page-form {
  display: inline-block;
  width: 100%;
  margin-top: 0px;
}

.contact-page-map {
  margin-top: 40px;
  margin-left: 25px;
}
.contact-page-form form {
  padding: 20px 15px 0;
}
</style>
