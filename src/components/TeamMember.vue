<script setup>
defineProps([
    'name',
    'designation',
    'avatar',
    'about'
])
</script>
<template>
   <div class="container">
    <div class="row">
        <div class="col-lg-12">
       <div class=" temp">
        <div class="">
            <a href="">
            <img :src="avatar" :alt="name">
        </a>
        </div>
        <div class="content">
            <h3 class="name">
               {{name}}
            </h3>
            <span class="designation "> {{designation}}</span>
            <p class="about"> {{about}}</p>
            <div class="col-lg-12">
            <div class="social-links mt-4">
                <a href="#"><i class="fa-brands fa-twitter"></i> </a>
                <a href="#"><i class="fa-brands fa-facebook"></i></a>
                <a href="#"><i class="fa-brands fa-skype"></i></a>
                <a href="#"><i class="fa-brands fa-linkedin"></i></a>
              </div>
            </div>
        </div>
       </div>
    </div>
    </div>
   </div>
      
</template>


<style scoped>
.temp{
    display: flex;
    /* justify-content: space-between; */
    justify-content: center;
    align-items: center;
    background-color: rgb(225, 240, 240);
    width: 100%;
    position: relative;
    
  
}
.content{
    padding: 30px;
   
   
}
.name{
    font-size: 2rem;
    font-weight: 400;
    color: rgb(57, 62, 62);
    line-height: 0.8;
    margin-top: 10px;
}
.designation{
    font: small;
    color: rgb(95, 101, 101);
   
}
.about{
    margin-top: 0px;
    text-align: left;
}

.social-links a {
  font-size: 18px;
  display: inline-block;
  
  line-height: 1;
  padding: 8px 0;
  margin-right: 4px;
  border-radius: 50%;
  text-align: center;
  width: 36px;
  height: 36px;
  transition: 0.3s;
}


.social-links a:hover {
  background-color: #1acc8d;
  color: #fff;
}

</style>