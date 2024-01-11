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
                <h2>address</h2>
                <span>1215 Lorem Ipsum, Ch 176080 </span>
                <span>Chandigarh , INDIA</span>
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
                <h2>E-mail</h2>
                <span>info@LoremIpsum.com</span>
                <span>yourmail@gmail.com</span>
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
                <h2>office time</h2>
                <span>Mon - Thu 9:00 am - 4.00 pm</span>
                <span>Thu - Mon 10.00 pm - 5.00 pm</span>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="row">
        <div class="col-md-8">
          <div class="contact-page-form" method="post">
            <form action="contact-mail.php" method="post">
              <div class="row">
                <div class="col-md-6 col-sm-6 col-xs-12">
                  <div class="single-input-field">
                    <input type="text" placeholder="Your Name" name="name" />
                  </div>
                </div>
                <div class="col-md-6 col-sm-6 col-xs-12">
                  <div class="single-input-field">
                    <input type="email" placeholder="E-mail" name="email" required />
                  </div>
                </div>
                <div class="col-md-6 col-sm-6 col-xs-12">
                  <div class="single-input-field">
                    <input type="text" placeholder="Phone Number" name="phone" />
                  </div>
                </div>
                <div class="col-md-6 col-sm-6 col-xs-12">
                  <div class="single-input-field">
                    <input type="text" placeholder="Subject" name="subject" />
                  </div>
                </div>
                <div class="col-md-12 message-input">
                  <div class="single-input-field">
                    <textarea placeholder="Write Your Message" name="message"></textarea>
                  </div>
                </div>
                <div class="single-input-fieldsbtn">
                  <input type="submit" value="Send Now" />
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

<script></script>

<style>

.loader {
    width: 100%;
    height: 100%;
    background-color: #333;
    position: absolute;
    top: 0;
    left: 0;
    -webkit-animation: loader 0.5s 2.2s ease forwards;
    animation: loader 0.5s 2.2s ease-in forwards;
    z-index: 99;
}

.progress-bar {
    width: 200px;
    height: 2px;
    background-color: #666;
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
    border-left: 0px solid #ccc;
    -webkit-animation: progress 2s ease-in-out forwards;
    animation: progress 2s ease-in-out forwards;
}

@-webkit-keyframes loader {
    to {left: -100%;}
}

@keyframes loader {
    to {left: -100%;}
}

@-webkit-keyframes progress {
    to {border-left: 200px solid #ccc;}
}

@keyframes progress {
    to {border-left: 200px solid #ccc;}
}

/* page loader */

section {
  padding: 10px;
  height: 950px;
}
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
  background: #071c34;
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
  background: #071c34;
  width: 150px;
  border-color: #071c34;
}
.contact-info-icon i {
  font-size: 48px;
  color: #fda40b;
}
.contact-info-text p {
  margin-bottom: 0px;
}
.contact-info-text h2 {
  color: #fff;
  font-size: 22px;
  text-transform: capitalize;
  font-weight: 600;
  margin-bottom: 10px;
}
.contact-info-text span {
  color: #999999;
  font-size: 16px;
  display: inline-block;
  width: 100%;
}

.contact-page-form input {
  background: #f9f9f9 none repeat scroll 0 0;
  border: 1px solid #f9f9f9;
  margin-bottom: 20px;
  padding: 12px 16px;
  width: 100%;
  border-radius: 4px;
}

.contact-page-form .message-input {
  display: inline-block;
  width: 100%;
  padding-left: 0;
}
.single-input-field textarea {
  background: #f9f9f9 none repeat scroll 0 0;
  border: 1px solid #f9f9f9;
  width: 100%;
  height: 120px;
  padding: 12px 16px;
  border-radius: 4px;
}
.single-input-fieldsbtn input[type="submit"] {
  background: #fda40b none repeat scroll 0 0;
  color: #fff;
  display: inline-block;
  font-weight: 600;
  padding: 10px 0;
  text-transform: capitalize;
  width: 150px;
  margin-top: 20px;
  font-size: 16px;
}
.single-input-fieldsbtn input[type="submit"]:hover {
  background: #071c34;
  transition: all 0.4s ease-in-out 0s;
  border-color: #071c34;
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
