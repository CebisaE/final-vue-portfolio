<template>
   <section id="contact" class="contact">
      <div class="container" data-aos="fade-up">

        <div class="section-title">
          <h2>Contact</h2>
        </div>

        <div class="row mt-1">

          <div class="col-lg-4">
            <div class="info">
              <div class="address">
                <i class="fa fa-map-pin" aria-hidden="true"></i>
                <h4>Location:</h4>
                <p>Cape Town, South Africa</p>
              </div>

              <div class="email">
                <i class="fa fa-envelope" aria-hidden="true"></i>
                <h4>Email:</h4>
                <p>mihlekcebisa@gmail.com</p>
              </div>

              <div class="phone">
                <i class="fa fa-phone" aria-hidden="true"></i>
                <h4>Call:</h4>
                <p>+27 74 737 7043</p>
              </div>

            </div>

          </div>

          <div class="col-lg-8 mt-5 mt-lg-0">

            <form action="https://formspree.io/f/mayvderw" method="post" role="form" target="_blank" class="email-form">
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
              <div class="text-center"><button type="submit">Send Message</button></div>
            </form>

          </div>

        </div>

      </div>
    </section><!-- End Contact Section -->
 <a href="#" class="back-to-top d-flex align-items-center justify-content-center"><i class="fa fa-arrow-up"></i></a>
</template>

<script>

</script>

<style scoped>
.contact{
    background-color: #f5f8fd;
}
.contact .info {
  width: 100%;
 background-color: #f5f8fd;

}
.contact .info i {
  font-size: 20px;
  color: #0563bb;
  float: left;
  width: 44px;
  height: 44px;
  background: #eef7ff;
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
  color: #45505b;
}
.contact .info p {
  padding: 0 0 0 60px;
  margin-bottom: 0;
  font-size: 14px;
  color: #728394;
}
.contact .info .email, .contact .info .phone {
  margin-top: 40px;
}
.contact .info .email:hover i, .contact .info .address:hover i, .contact .info .phone:hover i {
  background: #0563bb;
  color: #f5f8fd;;
}
.contact .email-form {
  width: 100%;
  background:#f5f8fd;;
}
.contact .email-form .form-group {
  padding-bottom: 8px;
}
.contact .email-form .error-message {
  display: none;
  color: #fff;
  background: #ed3c0d;
  text-align: left;
  padding: 15px;
  font-weight: 600;
}
.contact .email-form .error-message br + br {
  margin-top: 25px;
}
.contact .email-form .sent-message {
  display: none;
  color: #fff;
  background: #18d26e;
  text-align: center;
  padding: 15px;
  font-weight: 600;
}
.contact .email-form .loading {
  display: none;
  background: #fff;
  text-align: center;
  padding: 15px;
}
.contact .email-form .loading:before {
  content: "";
  display: inline-block;
  border-radius: 50%;
  width: 24px;
  height: 24px;
  margin: 0 10px -6px 0;
  border: 3px solid #18d26e;
  border-top-color: #eee;
  -webkit-animation: animate-loading 1s linear infinite;
  animation: animate-loading 1s linear infinite;
}
.contact .email-form input, .contact .email-form textarea {
  border-radius: 4px;
  box-shadow: none;
  font-size: 14px;
}
.contact .email-form input {
  height: 44px;
}
.contact .email-form textarea {
  padding: 10px 12px;
}
.contact .email-form button[type=submit] {
  background: #0563bb;
  border: 0;
  padding: 10px 35px;
  color: #fff;
  transition: 0.4s;
  border-radius: 50px;
}
.contact .email-form button[type=submit]:hover {
  background: #0678e3;
}
@-webkit-keyframes animate-loading {
  0% {
    transform: rotate(0deg);
  }
  100% {
    transform: rotate(360deg);
  }
}
@keyframes animate-loading {
  0% {
    transform: rotate(0deg);
  }
  100% {
    transform: rotate(360deg);
  }
}
.back-to-top {
  position: fixed;
  /* visibility: hidden;
  opacity: 0; */
  right: 15px;
  bottom: 15px;
  z-index: 996;
  background: #149ddd;
  width: 40px;
  height: 40px;
  border-radius: 50px;
  transition: all 0.4s;
}
.back-to-top i {
  font-size: 28px;
  color: #fff;
  line-height: 0;
}
.back-to-top:hover {
  background: #2eafec;
  color: #fff;
}
.back-to-top.active {
  visibility: visible;
  opacity: 1;
}

</style>