<script setup>
import TeamMember from './TeamMember.vue';
const title="Our Team";
const description="Explore the whole collection of open-source web components and <br/>elements built with the utility classes from Bootstrap"
</script>
<template>
   <section id="team-section">
   <div class="container">
    <div class="team-top">
        <h1 class="title">{{title}}</h1>
        <p v-html="description" class="descrptioni"></p>
    </div>
    
    
        <div class="team-member">
            <div class="row ">
                <div class="col-lg-6 col-md-12">
                    <TeamMember name="Bonnie Green " designation="CEO & Web Developer" avatar="//flowbite.s3.amazonaws.com/blocks/marketing-ui/avatars/bonnie-green.png" about="Bonnie drives the technical strategy of the flowbite platform and brand."/>
                </div>
                <div class="col-lg-6 col-md-12 ">
                    <TeamMember name="Jese Leos" designation="CTO" avatar="//flowbite.s3.amazonaws.com/blocks/marketing-ui/avatars/joseph-mcfall.png" about="Jese drives the technical strategy of the flowbite platform and brand."/>
                </div>
            </div>
    </div>
        <div class="team-member mt-5 mb-5">
            <div class="row">
                <div class="col-lg-6">
                    <TeamMember name="Michael Gough" designation="Senior Front-end Developer" avatar="//flowbite.s3.amazonaws.com/blocks/marketing-ui/avatars/michael-gouch.png" about="Michael drives the technical strategy of the flowbite and brand."/>
                </div>
                <div class="col-lg-6">
                    <TeamMember name="Lana Byrd" designation="Senior Back-end Developer" avatar="//flowbite.s3.amazonaws.com/blocks/marketing-ui/avatars/sofia-mcguire.png" about="Lana drives the technical strategy of the flowbite platform and brand."/>
                </div>
            </div>
        </div>
    
    
   </div>

   </section>

</template>
<style scoped>
#team-section{
    display: flex;
    background-color: #fff;
}
.team-top{
    margin:60px 0px 50px 0px;
    text-align: center;  
}
.title{
    font-size: 2.5rem;
    color: rgb(80, 93, 93);
    font-weight: bold;
}
.descrptioni{
    color: rgb(107, 130, 130);
    font-size: 1.5rem;

}


.team-member{
    display: flex;
    
}
</style>