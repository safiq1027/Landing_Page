<script setup>
  const title = 'Check The Features'
  const subTitle = 'Features'
  const box1Title = 'Easily Manage'
  const box2Title = 'Get Payments Easily'
  const box3Title = 'Quick Messaging'

  const box4Title = 'Easily Manage'
  const box5Title = 'Get Payments Easily'
  const box6Title = 'Quick Messaging'

  const box7Title = 'Easily Manage'
  const box8Title = 'Get Payments Easily'
  const box9Title = 'Quick Messaging'

  const box10Title = 'Easily Manage'
  const box11Title = 'Get Payments Easily'
  const box12Title = 'Quick Messaging'

</script>
<template>

    <section id="features" class="features">
      <div class="container">

        <div class="section-title">
          <h2>{{ subTitle }}</h2>
          <p>{{ title }}</p>
        </div>

        <div id="animation" class="row">
          <div class="col-lg-3 col-md-4">
            <div class="icon-box">
              <i class="fa-solid fa-store" style="color: #ffbb2c;"></i>
              <h3><a href="">{{ box1Title }}</a></h3>
            </div>
          </div>
          <div class="col-lg-3 col-md-4 mt-4 mt-md-0">
            <div class="icon-box">
              <i class="fa-solid fa-chart-simple" style="color: #5578ff;"></i>
              <h3><a href="">{{ box2Title }}</a></h3>
            </div>
          </div>
          <div class="col-lg-3 col-md-4 mt-4 mt-md-0">
            <div class="icon-box" data-aos="zoom-in" data-aos-delay="150">
              <i class="fa-solid fa-calendar-days" style="color: #e80368;"></i>
              <h3><a href="">{{ box3Title }}</a></h3>
            </div>
          </div>
          <div class="col-lg-3 col-md-4 mt-4 mt-lg-0">
            <div class="icon-box">
              <i class="fa-solid fa-paint-roller" style="color: #e361ff;"></i>
              <h3><a href="">{{ box4Title }}</a></h3>
            </div>
          </div>
          <div class="col-lg-3 col-md-4 mt-4">
            <div class="icon-box">
              <i class="fa-solid fa-database" style="color: #47aeff;"></i>
              <h3><a href="">{{ box5Title }}</a></h3>
            </div>
          </div>
          <div class="col-lg-3 col-md-4 mt-4">
            <div class="icon-box">
              <i class="fa-solid fa-circle-info" style="color: #ffa76e;"></i>
              <h3><a href="">{{ box6Title }}</a></h3>
            </div>
          </div>
          <div class="col-lg-3 col-md-4 mt-4">
            <div class="icon-box">
              <i class="fa-regular fa-file" style="color: #11dbcf;"></i>
              <h3><a href="">{{ box7Title }}</a></h3>
            </div>
          </div>
          <div class="col-lg-3 col-md-4 mt-4">
            <div class="icon-box" >
              <i class="fa-solid fa-tag" style="color: #4233ff;"></i>
              
              <h3><a href="">{{ box8Title }}</a></h3>
            </div>
          </div>
          <div class="col-lg-3 col-md-4 mt-4">
            <div class="icon-box">
              <i class="fa-solid fa-anchor" style="color: #b2904f;"></i>
              <h3><a href="">{{ box9Title }}</a></h3>
            </div>
          </div>
          <div class="col-lg-3 col-md-4 mt-4">
            <div class="icon-box" >
              <i class="fa-solid fa-tape" style="color: #b20969;"></i>
              <h3><a href="">{{ box10Title }}</a></h3>
            </div>
          </div>
          <div class="col-lg-3 col-md-4 mt-4">
            <div class="icon-box">
              <i class="fa-solid fa-wifi" style="color: #ff5828;"></i>
              <h3><a href="">{{ box11Title }}</a></h3>
            </div>
          </div>
          <div class="col-lg-3 col-md-4 mt-4">
            <div class="icon-box">
              <i class="fa-solid fa-fingerprint" style="color: #29cc61;"></i>
              <h3><a href="">{{ box12Title }}</a></h3>
            </div>
          </div>
        </div>

      </div>
    </section>

</template>
<style scoped>
.section-title{
    text-align: center;
    margin: 50px 0px 30px 0px;
}
.section-title h2{
    font-size: 2.5rem;
    color: rgb(120, 115, 115);
    font-weight: bold;
}
.section-title p{
    font-size: 1.2rem;
    color: rgb(100, 99, 99);
}
.features .icon-box {
  display: flex;
  align-items: center;
  padding: 20px;
  background: #f5f5ff;
}

.features .icon-box i {
  font-size: 32px;
  padding-right: 10px;
  line-height: 1;
}

.features .icon-box h3 {
  font-weight: 700;
  margin: 0;
  padding: 0;
  line-height: 1;
  font-size: 16px;
}

.features .icon-box h3 a {
  color: #010483;
  transition: ease-in-out 0.3s;
  text-decoration: none;
}

.features .icon-box h3 a:hover {
  color: #01036f;
}

.features .icon-box:hover {
  background: #ebebff;
}
#animation{
  position: relative;
  animation-name:features;
  animation-duration: 3s;  
  animation-fill-mode: forwards;

}
@keyframes features {
  from {top:200px;}
  to {top: 0px; }
}
</style>