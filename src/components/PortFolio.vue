<script setup>
const title = "Our Portfolio";
const subTitle = "Neque porro quisquam est,qui dolerum ipsum quia dolor sit amet <br>consectetur, adipisci velit,sed quia non numquam";
const btn1 = "ALL";
const btn2 = "WEB";
const btn3 = "APPS";
const btn4 = "ICONS";
const imageTitle1 = "ISOMETRIC PERSPECTIVE MOCK-UP";
const imageTitle2 = "TIME ZONE APP UI";
const imageTitle3 = "VIRO MEDIA PLAYERS UI";
const imageTitle4 = "BLOG / MAGAZINE FLAT UI KIT";
const loader = "LOAD MORE PROJECTS";

</script>
<template>
      <section id="portfolio">
                <h4>{{ title }}</h4>
                <P v-html="subTitle" class="portfolio-section-para1"></P>
                <div class="button">
                    <button class="btn"> <a href="#">{{btn1}}</a></button>
                    <button class="btn"> <a href="#">{{btn2}}</a></button>
                    <button class="btn"> <a href="#">{{btn3}}</a></button>
                    <button class="btn"> <a href="#">{{btn4}}</a></button>
                </div>
                <div class="row mt-5">
                    <div id="animation1" class="col-lg-6">
                        <img src="../assets/images/1.png" alt="first Photo">
                        <p class="port-section-para2 mt-3">{{imageTitle1}}</p>

                    </div>
                    <div id="animation2" class="col-lg-6">
                        <img src="../assets/images/2.png" alt="Second Photo">
                        <p class="port-section-para2 mt-3">{{imageTitle2}}</p>
                    </div>
                </div>
                <div class="row mt-5">
                    <div id="animation3" class="col-lg-6">
                        <img src="../assets/images/3.png" alt="3rd Photo">
                        <p class="port-section-para2 mt-3">{{imageTitle3}}</p>

                    </div>
                    <div id="animation4" class="col-lg-6">
                        <img src="../assets/images/4.png" alt="4th Photo">
                        <p class="port-section-para2 mt-3">{{imageTitle4}}</p>
                    </div>
                </div>
                <div class="port-submit">
                    <p class="mt-2">{{loader}}</p>
                </div>
             </section>

</template>
<style scoped>
#portfolio{
    background-color: #fff;
    padding: 100px;
    
 
}
#portfolio h4{
    text-align: center;
}

.portfolio-section-para1{
    text-align: center;
    color: rgb(65, 63, 63);

}
.button{
    display: flex;
    justify-content: center;
}
.btn:hover{
    background-color: rgb(172, 172, 172);
}
.button a{
  text-decoration: none;
}

.port-section-para2{
    text-align: center;
    color: rgb(80, 78, 78);
}
.port-submit{
    width: 300px;
    background-color: #0fcfac;
    color: white;
    padding: 5px;
    text-align: center;
    margin: 0 auto;
    font-size: 1.2rem;
    font-weight: bolder;
    border-radius: 5px;
    box-shadow: 1px 2px 4px #0fcfac;
}
.port-submit:hover{
    background-color: #1bbd9f;
    transition: o.3s;
}
#animation1{
  position: relative;
  animation-name:portfolio1;
  animation-duration: 3s;  
  animation-fill-mode: forwards;
}
@keyframes portfolio1 {
  from {top:200px;}
  to {top: 0px; }
}
#animation2{
  position: relative;
  animation-name:portfolio2;
  animation-duration: 3s;  
  animation-fill-mode: forwards;

}
@keyframes portfolio2 {
  from {top:200px;}
  to {top: 0px; }
}
#animation3{
  position: relative;
  animation-name:portfolio3;
  animation-duration: 3s;  
  animation-fill-mode: forwards;

}
@keyframes portfolio3 {
  from {top:-200px;}
  to {top: 0px; }
}
#animation4{
  position: relative;
  animation-name:portfolio4;
  animation-duration: 3s;  
  animation-fill-mode: forwards;

}
@keyframes portfolio4 {
  from {top:-200px;}
  to {top: 0px; }
}
</style>