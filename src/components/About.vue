<script setup>
  const title = 'Grat Application Ever'
  const description = 'Lorem ipsum dolor sit amet, consectetur adipiing elit, sed do eiusmod tempor incididunt ut labore et laborused sed do eiusmod tempor incididunt ut labore et laborused.'
  const box1Title = 'Easy to Costomize'
  const box1Description = 'Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry s standard dummy text ever since the 1500s'

  const box2Title = 'Extreme Security'
  const box2Description = 'Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry s standard dummy text ever since the 1500s'

  const box3Title = 'Customer Support'
  const box3Description = 'Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry s standard dummy text ever since the 1500s'
</script>

<template>

    <section id="about" class="about">
      <div class="container-fluid">

        <div class="row">
          <div id="imageAnimation" class="col-xl-5 col-lg-6 aboutImage">
            <a href="">
                <img src="../assets/images/about.png" alt="About Image" >
            </a>
          </div>

          <div id="textAnimation" class="col-xl-7 col-lg-6 icon-boxes d-flex flex-column align-items-stretch justify-content-center py-5 px-lg-5">
            <h3>{{ title }}</h3>
            <p>{{ description }}</p>

            <div class="icon-box">
              <div class="icon"><i class="fa-solid fa-fingerprint"></i></div>
              <h4 class="title"><a href="">{{ box1Title }}</a></h4>
              <p class="description">{{ box1Description }}</p>
            </div>

            <div class="icon-box">
              <div class="icon"><i class="fa-solid fa-gift"></i></div>
              <h4 class="title"><a href="">{{ box2Title }}</a></h4>
              <p class="description">{{ box2Description }}</p>
            </div>

            <div class="icon-box">
              <div class="icon"><i class="fa-solid fa-atom"></i></div>
              <h4 class="title"><a href="">{{ box3Title }}</a></h4>
              <p class="description">{{ box3Description }}</p>
            </div>

          </div>
        </div>
      </div>
    </section>

</template>

<style>
.about {
  padding: 40px 0 0 0;
}
.aboutImage{
    display: flex;
    justify-content: center;
    align-items: center;  
}
.aboutImage img{
   max-width: 700px;
   padding-left: 50px;
}

.about .icon-boxes h3 {
  font-size: 28px;
  font-weight: 700;
  color: #010483;
  margin-bottom: 15px;
}

.about .icon-box {
  margin-top: 40px;
}

.about .icon-box .icon {
  float: left;
  display: flex;
  align-items: center;
  justify-content: center;
  width: 64px;
  height: 64px;
  border: 2px solid #7ceec6;
  border-radius: 50px;
  transition: 0.5s;
}

.about .icon-box .icon i {
  color: #1acc8d;
  font-size: 32px;
}

.about .icon-box:hover .icon {
  background: #1acc8d;
  border-color: #1acc8d;
}

.about .icon-box:hover .icon i {
  color: #fff;
}

.about .icon-box .title {
  margin-left: 85px;
  font-weight: 700;
  margin-bottom: 10px;
  font-size: 18px;
}

.about .icon-box .title a {
  color: #343a40;
  transition: 0.3s;
}

.about .icon-box .title a:hover {
  color: #1acc8d;
}

.about .icon-box .description {
  margin-left: 85px;
  line-height: 24px;
  font-size: 14px;
}
a{
  text-decoration: none;
}
#imageAnimation{
  position: relative;
  animation-name:image;
  animation-duration: 5s;  
  animation-fill-mode: forwards;

}
@keyframes image {
  from {top:200px;}
  to {top: 0px; }
}
#textAnimation{
  position: relative;
  animation-name:text;
  animation-duration: 5s;  
  animation-fill-mode: forwards;

}
@keyframes text {
  from {top:-200px;}
  to {top: 0px; }
}
 
</style>