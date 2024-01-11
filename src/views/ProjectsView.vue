<template>
  <div class="project">
    <h1>My Projects:</h1>
  </div>
  <section class="wwww">
    <div class="container">
      <div class="row mt-5">
        <div class="col">
          <div class="card-container" id="demo">
            <div class="cardww" tabindex="0">
              <h2>JS E-Commerce Website:</h2>
              <img
                src="https://42f2671d685f51e10fc6-b9fcecea3e50b3b59bdc28dead054ebc.ssl.cf5.rackcdn.com/illustrations/fast_car_p4cu.svg"
                width="100%"
              />
            </div>
            <div class="cardww" tabindex="0">
              <h2>Hex To Rgb Converter:</h2>
              <img
                src="https://42f2671d685f51e10fc6-b9fcecea3e50b3b59bdc28dead054ebc.ssl.cf5.rackcdn.com/illustrations/business_shop_qw5t.svg"
                width="100%"
              />
            </div>
            <div class="cardww" tabindex="0">
              <h2>Rgb  to Hex Converter:</h2>
              <img
                src="https://42f2671d685f51e10fc6-b9fcecea3e50b3b59bdc28dead054ebc.ssl.cf5.rackcdn.com/illustrations/apartment_rent_o0ut.svg"
                width="100%"
              />
            </div>
            <div class="cardww" tabindex="0">
              <h2>Js Calculator:</h2>
              <img
                src="https://42f2671d685f51e10fc6-b9fcecea3e50b3b59bdc28dead054ebc.ssl.cf5.rackcdn.com/illustrations/work_time_lhoj.svg"
                width="100%"
              />
            </div>
            <div class="cardww" tabindex="0">
              <h2>Netflix Cloned Website:</h2>
              <img
                src="https://42f2671d685f51e10fc6-b9fcecea3e50b3b59bdc28dead054ebc.ssl.cf5.rackcdn.com/illustrations/doctors_hwty.svg"
                width="100%"
              />
            </div>
            <div class="cardww" tabindex="0">
              <h2>YouTube Cloned Website:</h2>
              <img
                src="https://42f2671d685f51e10fc6-b9fcecea3e50b3b59bdc28dead054ebc.ssl.cf5.rackcdn.com/illustrations/exams_g4ow.svg"
                width="100%"
              />
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script></script>

<style>

.card-container {
  display: flex;
  padding: 2rem 1rem;
}
.card-container .cardww {
  flex: 1;
  transition: all 0.3s ease-in-out;
  background-color: #333;
  color: gold;
  padding: 15px;
  border-radius: 10px;
  box-shadow: 0 0 15px 0px rgba(0, 0, 0, 0.2);
}
.cardww h2 {
  font-size: 22px;
}
.card-container .cardww:not(:first-child) {
  margin-left: -10rem;
}
.cardww img {
  padding: 35px;
  width: 220px;
  display: block;
  margin: 0 auto;
}
.card-container .cardww:hover,
.card-container .cardww:focus {
  transform: translateY(3rem);
  outline: none;
}
.card-container .cardww:hover ~ .cardww,
.card-container .cardww:focus ~ .cardww {
  transform: translateX(10.5rem);
}

@media (max-width: 767px) {
  #demo {
    margin-top: 0px;
  }

  .card-container {
    flex-wrap: wrap;
    justify-content: center;
    padding: 0rem 1rem 2rem;
  }
  .card-container .cardww {
    flex: 1 1 100%;
    max-width: 200px;
  }
  .card-container .cardww:not(:first-child) {
    margin-left: 0rem;
    margin-top: 2rem;
  }
  .card-container .cardww:hover,
  .card-container .cardww:focus {
    transform: translateX(0rem);
  }
  .card-container .cardww:hover ~ .cardww,
  .card-container .cardww:focus ~ .cardww {
    transform: translateY(0rem);
  }
  .cardww img {
    padding: 5px;
  }
}
</style>
