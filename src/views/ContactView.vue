<template>
  <div id="Contact">
    <h1>Contact Me</h1>
    <br>
    <section class="contact-page-sec">
      <div class="container">
        <div class="row">
          <div class="col-md-8">
            <div class="contact-page-form">
              <form
                @submit.prevent="submitForm"
                method="post"
                action="https://formspree.io/f/xleqdjjr"
              >
                <div class="row">
                  <div class="col-md-6 col-sm-6 col-xs-12">
                    <div class="single-input-field">
                      <input
                        type="text"
                        placeholder="Your Name"
                        name="name"
                        v-model="formData.name"
                        required
                      />
                    </div>
                  </div>
                  <div class="col-md-6 col-sm-6 col-xs-12">
                    <div class="single-input-field">
                      <input
                        type="email"
                        placeholder="E-mail"
                        name="email"
                        v-model="formData.email"
                        required
                      />
                    </div>
                  </div>
                  <div class="col-md-6 col-sm-6 col-xs-12">
                    <div class="single-input-field">
                      <input
                        type="text"
                        placeholder="Phone Number"
                        name="phone"
                        v-model="formData.message"
                        required
                      />
                    </div>
                  </div>
                  <div class="col-md-12 message-input">
                    <div class="single-input-field">
                      <textarea
                        placeholder="Write Your Message"
                        name="message"
                      ></textarea>
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
                width="800"
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
  </div>
</template>

<script>
// @ is an alias to /src

import axios from "axios";
export default {
  components: {},
  data() {
    return {
      formData: {
        name: "",
        email: "",
        message: "",
        phone: "",
      },
    };
  },
  methods: {
    async submitForm() {
      try {
        // You can add form validation logic here if needed
        console.log("Form submitted with data:", this.formData);
        // If you want to send an AJAX request, you can use libraries like Axios
        // Example using Axios:
        await axios.post("https://formspree.io/f/xleqdjjr", this.formData);
        // Reset the form after submission
        this.formData = {
          name: "",
          email: "",
          message: "",
        };
      } catch (error) {
        console.error("Error submitting form:", error);
      }
    },
  },
};
</script>

<style scoped>

.contact-info {
  display: flex;
  text-align: center;
  margin-bottom: 10px;
}
.contact-info-icon {
  margin-bottom: 15px;
}
.contact-info-item {
  background: gold;
  border-radius: 50px;
  width: 200px;
  padding: 50px 50px;
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
  border-color: black;
}
.contact-info-icon i {
  font-size: 48px;
  color: gold;
}
.contact-info-text p {
  margin-bottom: 0px;
}
.contact-info-text h1 {
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
  width: 500px;
  border-radius: 40px;
}

.contact-page-form .message-input {
  display: inline-block;
  width: 600px;
  padding-left: 0;
}
.single-input-field textarea {
  background: #ddd none repeat scroll 0 0;
  border: 2px solid #000;
  width: 500px;
  height: 120px;
  padding: 12px 16px;
  border-radius: 20px;
}
.single-input-fieldsbtn button[type="submit"] {
  background: #111 none repeat scroll 0 0;
  border-radius: 50px;
  color: gold;
  display: inline-block;
  font-weight: 600;
  padding: 10px 0;
  text-transform: capitalize;
  width: 150px;
  margin-top: 20px;
  font-size: 16px;
  transition: all 0.7s ease-in-out 0s;
}
.single-input-fieldsbtn button[type="submit"]:hover {
  background: gold;
  color: black;
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
