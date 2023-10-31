<script setup>
const title = "Contact Us";
const subTitle = "Lorem ipsum dolor sit amet consectetur adipisicing elit.  Adipisci  expedita.<br> officiis  culpa earum  earum fugiat quo!"
;
const location = "652 kazipara,Mirpur-10,Dhaka";
const email = "safiq1027@gmail.com";
const mobileNumber = "01634087120"
</script>
<template>
    <section id="contact" class="contact">
        <div class="container">
            <div class="section-title">
                <h2 class="title">{{title}} </h2>
                <p v-html="subTitle" class="sub-title"></p>
            </div>
            <div class="row">
                <div class="col-lg-4 addressAnimation">
                    <div class="info">
                        <div class="address">
                            <i class="fa-solid fa-location-dot"></i>
                            <h4>Location:</h4>
                            <p>{{ location }}</p>
                        </div>
                        <div class="email">
                            <i class="fa-regular fa-envelope"></i>
                            <h4>Email:</h4>
                            <p>{{email}}</p>
                        </div>

                        <div class="phone">
                            <i class="fa-solid fa-mobile"></i>
                            <h4>Call:</h4>
                            <p>{{mobileNumber}}</p>
                        </div>
                    </div>
                </div>
                <div class="col-lg-8 mt-5 mt-lg-0 fromAnimation" >

                    <form action="" method="" role="form" class="">
                        <div class="row">
                            <div class="col-md-6 form-group">
                            <input type="text" name="name" class="form-control" id="name" placeholder="Your Name" required>
                            </div>
                            <div class="col-md-6 form-group mt-3 mt-md-0">
                            <input type="email" class="form-control" name="email" id="email" placeholder="Your Email" required>
                            </div>
                        </div>
                        <div class="form-group mt-3">
                            <input type="text" class="form-control" name="subject" id="subject" placeholder="Subject" required>
                        </div>
                        <div class="form-group mt-3">
                            <textarea class="form-control" name="message" rows="5" placeholder="Message" required></textarea>
                        </div>
                        <div class=" text-center mb-5 mt-2"><button type="submit">Send Message</button></div>
                    </form>

                </div>

            </div>
        </div>
    </section>

</template>
<style scoped>
#contact{
  background-color: #fff;
}
.section-title{
  text-align: center;
}

.title{
    color: #707079;
    font-size: 2.5rem;
    font-weight:bold ;
    text-transform: capitalize;
}
.sub-title{
    color: rgb(113, 105, 105);
    font-size: 1.5rem;
    text-transform: capitalize;
    margin-bottom: 2rem;
}

.contact .info {
  width: 100%;
  background: #fff;
}

.contact .info i {
  font-size: 20px;
  color: #3f43fd;
  float: left;
  width: 44px;
  height: 44px;
  background: #f0f0ff;
  display: flex;
  justify-content: center;
  align-items: center;
  border-radius: 50px;
  transition: all 0.3s ease-in-out;
}

.contact .info h4 {
  padding: 0 0 0 60px;
  font-size: 22px;
  font-weight: 600;
  margin-bottom: 5px;
  color: #010483;
}

.contact .info p {
  padding: 0 0 0 60px;
  margin-bottom: 0;
  font-size: 14px;
  color: #0205a1;
}

.contact .info .email,
.contact .info .phone {
  margin-top: 40px;
}

.contact .info .email:hover i,
.contact .info .address:hover i,
.contact .info .phone:hover i {
  background: #1acc8d;
  color: #fff;
}

button{
    background-color:rgb(13, 193, 133);
    color: white;
    padding: 10px 30px;
    border-radius: 50px;
    border: none;
    transition:  0.3s;
}
button:hover{
    background-color: lightseagreen;
    
}
.addressAnimation{
  position: relative;
  animation-name:address;
  animation-duration: 3s;  
  animation-fill-mode: forwards;

}

@keyframes address {
  from {top:200px;}
  to {top: 0px; }
}
.fromAnimation{
  position: relative;
  animation-name:from;
  animation-duration: 5s;  
  animation-fill-mode: forwards;
}
@keyframes from {
  from {top:-200px;}
  to {top: 0px; }
}

</style>