<script setup>
  const logoTitle = 'Cuda'
  const  description = 'Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industrys standard dummy'
  const addressHtml = '652 kazipara <br>Mirpur-10, Dhaka<br><br><strong>Phone:</strong>+880 1634 087 120<br><strong>Email:</strong>safiq1027@gmail.com<br>'
  const copyRightHtml = '&copy; Copyright <strong><span>Safiq</span></strong>. All Rights Reserved'
  const designer = 'Designed by '
</script>

<template>
    <footer id="footer">
    <div class="footer-top">
      <div class="container">
        <div class="row">

          <div class="col-lg-4 col-md-6">
            <div class="footer-info">
              <h3>{{ logoTitle }}</h3>
              <p class="pb-3"><em>{{ description }}</em></p>
              <p v-html="addressHtml">
                
              </p>
              <div class="social-links mt-3">
                <a href="#"><i class="fa-brands fa-twitter"></i> </a>
                <a href="#"><i class="fa-brands fa-facebook"></i></a>
                <a href="#"><i class="fa-brands fa-skype"></i></a>
                <a href="#"><i class="fa-brands fa-linkedin"></i></a>
              </div>
            </div>
          </div>

          <div class="col-lg-2 col-md-6 footer-links">
            <h4>Useful Links</h4>
            <ul>
              <li><i class="fa-solid fa-angle-right"></i> <a href="#">Home</a></li>
              <li><i class="fa-solid fa-angle-right"></i> <a href="#">About us</a></li>
              <li><i class="fa-solid fa-angle-right"></i> <a href="#">Services</a></li>
              <li><i class="fa-solid fa-angle-right"></i> <a href="#">Terms of service</a></li>
              <li><i class="fa-solid fa-angle-right"></i> <a href="#">Privacy policy</a></li>
            </ul>
          </div>

          <div class="col-lg-2 col-md-6 footer-links">
            <h4>Our Services</h4>
            <ul>
              <li><i class="fa-solid fa-angle-right"></i> <a href="#">Web Design</a></li>
              <li><i class="fa-solid fa-angle-right"></i> <a href="#">Web Development</a></li>
              <li><i class="fa-solid fa-angle-right"></i> <a href="#">Product Management</a></li>
              <li><i class="fa-solid fa-angle-right"></i> <a href="#">Marketing</a></li>
              <li><i class="fa-solid fa-angle-right"></i> <a href="#">Graphic Design</a></li>
            </ul>
          </div>

          <div class="col-lg-4 col-md-6 footer-newsletter">
            <h4>Our Newsletter</h4>
            <p>Tamen quem nulla quae legam multos aute sint culpa legam noster magna</p>
            <form action="" method="post">
              <input type="email" name="email"><input type="submit" value="Subscribe">
            </form>

          </div>

        </div>
      </div>
    </div>

    <div class="container">
      <div class="copyright" v-html="copyRightHtml">
        
      </div>

      <div class="credits" >
        <p>{{ designer }} <a href="">Md Safiqul Islam</a></p>
      </div>
    </div>
  </footer>

</template>

<style scoped>
#footer {
  background: #010351;
  padding: 0 0 30px 0;
  color: #fff;
  font-size: 14px;
}

.footer-top {
  padding: 60px 0 30px 0;
}

 .footer-info {
  margin-bottom: 15px;
  background: #010246;
  color: #fff;
  border-top: 4px solid #61ddb2;
  text-align: center;
  padding: 30px 20px;
}

 .footer-info h3 {
  font-size: 24px;
  margin: 0 0 20px 0;
  padding: 2px 0 2px 0;
  line-height: 1;
  font-weight: 700;
}

.footer-info p {
  font-size: 14px;
  line-height: 24px;
  margin-bottom: 0;
  font-family: "Montserrat", sans-serif;
}

.footer-top .social-links a {
  font-size: 18px;
  display: inline-block;
  color: #fff;
  line-height: 1;
  padding: 8px 0;
  margin-right: 4px;
  border-radius: 50%;
  text-align: center;
  width: 36px;
  height: 36px;
  transition: 0.3s;
}


.footer-top .social-links a:hover {
  background-color: #1acc8d;
  color: #fff;
}


.footer-top h4 {
  font-size: 16px;
  font-weight: 600;
  color: #fff;
  position: relative;
  padding-bottom: 12px;
}

.footer-top .footer-links {
  margin-bottom: 30px;
  
}

#footer .footer-top .footer-links ul {
  list-style: none;
  padding: 0;
  margin: 0;
}
.footer-top .footer-links ul i {
  padding-right: 2px;
  color: #61ebba;
  font-size: 18px;
  line-height: 1;
}

.footer-top .footer-links ul li {
  padding: 10px 0;
  display: flex;
  align-items: center;
}

#footer .footer-top .footer-links ul li:first-child {
  padding-top: 0;
}

#footer .footer-top .footer-links ul a {
  color: #fff;
  transition: 0.3s;
  display: inline-block;
  line-height: 1;
}

#footer .footer-top .footer-links ul a:hover {
  color: #4be8b0;
}

#footer .footer-top .footer-newsletter form {
  margin-top: 30px;
  background: #fff;
  padding: 6px 10px 6px 15px;
  position: relative;
  border-radius: 50px;
}

#footer .footer-top .footer-newsletter form input[type=email] {
  border: 0;
  padding: 4px;
  width: calc(100% - 110px);
}

#footer .footer-top .footer-newsletter form input[type=submit] {
  position: absolute;
  top: 0;
  right: -2px;
  bottom: 0;
  border: 0;
  background: none;
  font-size: 16px;
  padding: 0 20px;
  background: #1acc8d;
  color: #fff;
  transition: 0.3s;
  border-radius: 50px;
}

#footer .footer-top .footer-newsletter form input[type=submit]:hover {
  background: #149f6e;
}

#footer .copyright {
  border-top: 1px solid #010479;
  text-align: center;
  padding-top: 30px;
}

#footer .credits {
  padding-top: 10px;
  text-align: center;
  font-size: 13px;
  color: #fff;
}
#footer a{
    text-decoration: none;
}

</style>