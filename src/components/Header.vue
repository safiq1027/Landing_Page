<script setup>

</script>

<template>
  <div class="header">

<nav class="navbar navbar-expand-md">
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNavDropdown" aria-controls="navbarNavDropdown" aria-expanded="false" aria-label="Toggle navigation">
        <span> <i class="fas fa-bars navbar-icon"></i> </span>
      </button>
      <a class="navbar-brand" href="#">
        <img src="../assets/images/logo.png" alt="logo">
    </a>
    <div class="collapse navbar-collapse" id="navbarNavDropdown">
        <ul class="navbar-nav ml-auto">
            <li class="nav-item">
                <a class="nav-link text-center text-md-left" href="#home">Home</a>
                
            </li>
            <li class="nav-item">
                <a class="nav-link text-center text-md-left" href="#about">About</a>
            </li>
            <li class="nav-item">
                <a class="nav-link text-center text-md-left" href="#features">features</a>
            </li>
            <li class="nav-item">
                <a class="nav-link text-center text-md-left" href="#gallery">Gallery</a>
            </li>
            <li class="nav-item">
                <a class="nav-link text-center text-md-left" href="#team-section">Team</a>
            </li>
            
            <li class="nav-item">
                <a class="nav-link text-center text-md-left" href="#portfolio">Blog</a>
            </li>
            <li class="nav-item">
                <a class="nav-link text-center text-md-left" href="#contact">Contact</a>
            </li>
        </ul>
    </div>
</nav>

</div>


</template>

<style scoped>
.header{
    background-color: 	#ba55d3;
    padding:5px;
    position: sticky;
    top: 0;
    z-index: 10000;
    
}
.header{
    background-image: url("images/laptop.jpg");
    background-position: center;
    background-attachment: fixed;
    background-repeat: no-repeat;
    background-size: cover;
}
.header .navbar{
    height: 55px;
}
.navbar-brand img{
    width: 100px;
    height: auto;
    margin: 0px 100px;
}
.nav-link{
    color: white;
    margin: 10px;
    border-radius: 5px;
    transition: 0.4s;
}
.navbar-nav{
    margin: 0px 100px;
}
.nav-link:hover{
   background-color: #2980b9;
   color: white;
   transform: scale(1.1);
}

</style>