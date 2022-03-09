<template>
  <section id="resume" class="resume">
      <div class="container">

        <div class="section-title">
          <h2>Resume</h2>
          <p>A little bit of my background</p>
        </div>

        <div class="row">
          <div class="col-lg-6" data-aos="fade-up">
            <h3 class="resume-title">Sumary</h3>
            <div class="resume-item pb-0">
              <h4>Emihle Cebisa</h4>
              <p><em>An Aspiring Fullstack Developer looking to increase their experience and  grow their skill</em></p>
              <ul class="list">
                <li>Cape Town,western cape, SA</li>
                <li>mihlekcebisa@gmail.com</li>
              </ul>
            </div>

            <h3 class="resume-title">Educational  Experience</h3>
            <div class="resume-item">
              <h4>National Senior Certificate</h4>
              <h5>2015</h5>
              <p><em>Luhlaza High School</em></p>
              <ul class="list">
                <li>Mathematics</li>
                <li>Life science</li>
                 <li>Physical science</li>
                  <li>Geography</li>
                   <li>Isixhosa Home Language</li>
                    <li>English First Additional Language</li>
                     <li>Life Orientation</li>
              </ul>
            </div>
          </div>
          <div class="col-lg-6" data-aos="fade-up" data-aos-delay="100">
            <h3 class="resume-title">Professional Experience</h3>
            <div class="resume-item">
              <h4>Aspiring Fullstack Developer</h4>
              <h5>2021 - Present</h5>
            <ul class="list">
                <li>HTML5</li>
                <li>CSS</li>
                 <li>BOOTSTRAP</li>
                  <li>MYSQL</li>
                   <li>JAVASCRIPT</li>
                    <li>NODE JS</li>
                     <li>VUE JS</li>
              </ul>
            </div>
             <h3 class="resume-title">Volunteering  Experience</h3>
            <div class="resume-item">
              <h4>Rise Young Women's Club </h4>
              <h5>2018</h5>
              <p><em>@ Luhlaza High School</em></p>
              <p><em>The goal of the Rise Young Womens clubs is to focus on and prioritise support for the rights and activism of young womxn.
                The clubs create a safe space for girls and young women to collectively advocate for issues that matter to them and affect them.</em></p>
            </div>
          </div>
        </div>

      </div>
    </section>
</template>
<script>

export default {
  name: 'Resume',
  components: {
  }
}
</script>

<style scoped>
.container {
  padding:5em;
}
.list{
  list-style-type: none;
}
.resume .resume-title {
  font-size: 26px;
  font-weight: 700;
  margin-top: 20px;
  margin-bottom: 20px;
  color: #050d18;
}
.resume .resume-item {
  padding: 0 0 20px 20px;
  margin-top: -2px;
  border-left: 2px solid #1f5297;
  position: relative;
}
.resume .resume-item h4 {
  line-height: 18px;
  font-size: 18px;
  font-weight: 600;
  text-transform: uppercase;
  font-family: "Poppins", sans-serif;
  color: #050d18;
  margin-bottom: 10px;
}
.resume .resume-item h5 {
  font-size: 16px;
  background: #e4edf9;
  padding: 5px 15px;
  display: inline-block;
  font-weight: 600;
  margin-bottom: 10px;
}
.resume .resume-item ul {
  padding-left: 20px;
}
.resume .resume-item ul li {
  padding-bottom: 10px;
}
.resume .resume-item:last-child {
  padding-bottom: 0;
}
.resume .resume-item::before {
  content: "";
  position: absolute;
  width: 16px;
  height: 16px;
  border-radius: 50px;
  left: -9px;
  top: 0;
  background: #fff;
  border: 2px solid #1f5297;
}
</style>