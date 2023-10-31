<script setup>
const text1="Hi there! We are the new kids on the block";
const text2="and we build awesome websites and mobile apps.";
const text3= "WORK WITH US!";
</script>
<template>
    <section id="home" class="head-para">
       <p>{{ text1 }} <br> {{ text2 }}</p>
        <p class="head-para1">{{ text3 }}</p>
    </section>

</template>
<style scoped>
.head-para{
    padding: 100px;
    text-align: center;
    color: white;
    font-size: 1.8rem;
    font-weight: bolder;
    background-color: 	#ba55d3;
}
.head-para1{
    background-color: orange;
    width: 300px;
    text-align: center;
    margin: 2.5rem auto;
    font-size: 1.5rem;
    padding: 10px;
    font-weight: normal;
    box-shadow: 1px 2px 4px orange;
    border-radius: 5px;
}
</style>