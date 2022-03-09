<template>
  <section id="about" class="about">
      <div class="container">

        <div class="section-title">
          <h2>About</h2>
          <p>A little bit information about me</p>
        </div>

        <div class="row">
          <div class="col-lg-4" data-aos="fade-right">
            <img src="https://i.postimg.cc/htbQPnYV/rsz-img-20220228-wa0028.jpg" class="img-fluid" alt="">
          </div>
          <div class="col-lg-8 pt-4 pt-lg-0 content" data-aos="fade-left">
            <h3>UI/UX Designer &amp; Web Developer.</h3>
            <p class="fst-italic">
            I am a hard-working, Ambivert who loves meeting new people
            and getting to know them.
            furthermore, I assist where I can, as I love helping others.
            </p>
            <div class="row">
              <div class="col-lg-6">
                <ul>
                  <li><i class="bi bi-chevron-right"></i> <strong>Birthday:</strong> <span>02 April 2002</span></li>
                  <li><i class="bi bi-chevron-right"></i> <strong>Phone:</strong> <span>+27 74 737 7043</span></li>
                  <li><i class="bi bi-chevron-right"></i> <strong>City:</strong> <span>Cape Town,SA</span></li>
                </ul>
              </div>
              <div class="col-lg-6">
                <ul>
                  <li><i class="bi bi-chevron-right"></i> <strong>Email:</strong> <span>mihlekcebisa@gmail.com</span></li>
                  <li><i class="bi bi-chevron-right"></i> <strong>Freelance:</strong> <span>Available</span></li>
                </ul>
              </div>
            </div>
            <p>
              My love for coding began a long time ago,
              just that I didn't have the opportunity to do coding
              A family friend introduced me to coding,
              when he told me to try out Lifechoices since he knew that
              I am interested in technology.
            </p>
          </div>
        </div>

      </div>
    </section><!-- End About Section -->
<section id="skills" class="skills section-bg">
      <div class="container">

        <div class="section-title">
          <h2>Skills</h2>
          <p>A small evaluation of the skills I learnt in Lifechoices </p>
        </div>

        <div class="row skills-content">

          <div class="col-lg-6" data-aos="fade-up">

            <div class="progress">
              <span class="skill">HTML <i class="val">100%</i></span>
              <div class="progress-bar-wrap">
                <div class="progress-bar" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100"></div>
              </div>
            </div>

            <div class="progress">
              <span class="skill">CSS <i class="val">90%</i></span>
              <div class="progress-bar-wrap">
                <div class="progress-bar" role="progressbar" aria-valuenow="90" aria-valuemin="0" aria-valuemax="100"></div>
              </div>
            </div>

            <div class="progress">
              <span class="skill">JavaScript <i class="val">75%</i></span>
              <div class="progress-bar-wrap">
                <div class="progress-bar" role="progressbar" aria-valuenow="75" aria-valuemin="0" aria-valuemax="100"></div>
              </div>
            </div>

          </div>

          <div class="col-lg-6" data-aos="fade-up" data-aos-delay="100">

            <div class="progress">
              <span class="skill">Vue <i class="val">80%</i></span>
              <div class="progress-bar-wrap">
                <div class="progress-bar" role="progressbar" aria-valuenow="80" aria-valuemin="0" aria-valuemax="100"></div>
              </div>
            </div>

            <div class="progress">
              <span class="skill">Mysql <i class="val">90%</i></span>
              <div class="progress-bar-wrap">
                <div class="progress-bar" role="progressbar" aria-valuenow="90" aria-valuemin="0" aria-valuemax="100"></div>
              </div>
            </div>

            <div class="progress">
              <span class="skill">Bootstrap <i class="val">55%</i></span>
              <div class="progress-bar-wrap">
                <div class="progress-bar" role="progressbar" aria-valuenow="55" aria-valuemin="0" aria-valuemax="100"></div>
              </div>
            </div>

          </div>

        </div>

      </div>
    </section>
</template>

<script>

export default {
  name: 'About',

}
</script>

<style scoped>
.container {
    padding:5em;
}
.about .content h3 {
  font-weight: 700;
  font-size: 26px;
  color: #173b6c;
}
.about .content ul {
  list-style: none;
  padding: 0;
}
.about .content ul li {
  margin-bottom: 20px;
  display: flex;
  align-items: center;
}
.about .content ul strong {
  margin-right: 10px;
}
.about .content ul i {
  font-size: 16px;
  margin-right: 5px;
  color:  #173b6c;
  line-height: 0;
}
.about .content p:last-child {
  margin-bottom: 0;
}
/* skills sections */

.skills .progress {
  height: 60px;
  display: block;
  background: none;
  border-radius: 0;
}
.skills .progress .skill {
  padding: 0;
  margin: 0 0 6px 0;
  text-transform: uppercase;
  display: block;
  font-weight: 600;
  font-family: "Poppins", sans-serif;
  color: #050d18;
}
.skills .progress .skill .val {
  float: right;
  font-style: normal;
  color: #149ddd;
}
.skills .progress-bar-wrap {
  background: #dce8f8;
  height: 10px;
}
.skills .progress-bar {
  width: 1px;
  height: 10px;
  transition: 0.9s;
  background-color: #149ddd;
}
</style>