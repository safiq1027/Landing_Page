<script setup>
import Carousal from './Carousal.vue';
const title = "Gallery";
const subTitle = "Lorem ipsum dolor sit amet consectetur adipisicing elit.  Adipisci  expedita.<br> officiis  culpa earum  earum fugiat quo!"
</script>
<template>
  <section id="gallery">
   <div class="title-section">
    <h3 class="title"> {{title}}</h3>
    <p v-html="subTitle" class="sub-title"></p>
   </div>
   <div>
    <Carousal/>
   </div>
  </section>
  

</template>
<style scoped>
#gallery{
  background-color: #fff;
}
.title-section{
  text-align: center;
  margin: 70px 0px 40px 0px;
}
.title{
  font-size: 2.5rem;
  font-weight: bold;
  color: rgb(95, 93, 93);
}
.sub-title{
  font-size: 1.5rem;
  color: gray;
}
</style>