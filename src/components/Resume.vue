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
              <ul>
                <li>Cape Town,western cape, SA</li>
                <li>mihlekcebisa@gmail.com</li>
              </ul>
            </div>

            <h3 class="resume-title">Educational  Experience</h3>
            <div class="resume-item">
              <h4>National Senior Certificate</h4>
              <h5>2015</h5>
              <p><em>Luhlaza High School</em></p>
              <ul>
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
              <p><em>Lifechoices Coding Academy </em></p>
              <p><em></em></p>
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

/* .resume{
    font-family: sans-serif;
    font-size: 7rem;
    font-weight: 700;
    color: #ea4343;
    letter-spacing: -.2px;
    display: inline-block;
    margin-bottom: 6px;
    padding-bottom:15px;
}
.main-timeline4 {
    overflow: hidden;
    position: relative
}

.main-timeline4:after,
.main-timeline4:before {
    content: "";
    display: block;
    width: 100%;
    clear: both
}

.main-timeline4:before {
    content: "";
    width: 3px;
    height: 100%;
    background: #d6d5d5;
    position: absolute;
    top: 30px;
    left: 50%
}

.main-timeline4 .timeline {
    width: 50%;
    float: left;
    padding-right: 30px;
    position: relative
}

.main-timeline4 .timeline-icon {
    width: 32px;
    height: 32px;
    border-radius: 50%;
    background: #fff;
    border: 3px solid #ea4343;
    position: absolute;
    top: 5.5%;
    right: -17.5px
}

.main-timeline4 .year {
    display: block;
    padding: 10px;
    margin: 0;
    font-size: 30px;
    color: #fff;
    border-radius: 0 50px 50px 0;
    background: #ea4343 ;
    text-align: center;
    position: relative
}

.main-timeline4 .year:before {
    content: "";
    border-top: 35px solid #ea4343 ;
    border-left: 35px solid transparent;
    position: absolute;
    bottom: -35px;
    left: 0
}

.main-timeline4 .timeline-content {
    padding: 30px 20px;
    margin: 0 45px 0 35px;
    background: #f2f2f2
}

.main-timeline4 .title {
    font-size: 19px;
    font-weight: 700;
    color: #504f54;
    margin: 0 0 10px
}

.main-timeline4 .description {
    font-size: 14px;
    color: #7d7b7b;
    margin: 0
}

.main-timeline4 .timeline:nth-child(2n) {
    padding: 0 0 0 30px
}

.main-timeline4 .timeline:nth-child(2n) .timeline-icon {
    right: auto;
    left: -14.5px
}

.main-timeline4 .timeline:nth-child(2n) .year {
    border-radius: 50px 0 0 50px;
    background: #7d7d7d
}

.main-timeline4 .timeline:nth-child(2n) .year:before {
    border-left: none;
    border-right: 35px solid transparent;
    left: auto;
    right: 0
}

.main-timeline4 .timeline:nth-child(2n) .timeline-content {
    text-align: right;
    margin: 0 35px 0 45px
}

.main-timeline4 .timeline:nth-child(2) {
    margin-top: 170px
}

.main-timeline4 .timeline:nth-child(odd) {
    margin: -175px 0 0
}

.main-timeline4 .timeline:nth-child(even) {
    margin-bottom: 80px
}

.main-timeline4 .timeline:first-child,
.main-timeline4 .timeline:last-child:nth-child(even) {
    margin: 0
}

.main-timeline4 .timeline:nth-child(2n) .timeline-icon {
    border-color: #7d7d7d
}

.main-timeline4 .timeline:nth-child(2n) .year:before {
    border-top-color: #7d7d7d
}

.main-timeline4 .timeline:nth-child(3n) .timeline-icon {
    border-color: #ea4343
}

.main-timeline4 .timeline:nth-child(3n) .year {
    background: #ea4343
}

.main-timeline4 .timeline:nth-child(3n) .year:before {
    border-top-color: #ea4343
}

.main-timeline4 .timeline:nth-child(4n) .timeline-icon {
    border-color: #7d7d7d
}

.main-timeline4 .timeline:nth-child(4n) .year {
    background: #7d7d7d
}

.main-timeline4 .timeline:nth-child(4n) .year:before {
    border-top-color: #7d7d7d
}

@media only screen and (max-width:767px) {
    .main-timeline4 {
        overflow: visible
    }
    .main-timeline4:before {
        top: 0;
        left: 0
    }
    .main-timeline4 .timeline:nth-child(2),
    .main-timeline4 .timeline:nth-child(even),
    .main-timeline4 .timeline:nth-child(odd) {
        margin: 0
    }
    .main-timeline4 .timeline {
        width: 100%;
        float: none;
        padding: 0 0 0 30px;
        margin-bottom: 20px!important
    }
    .main-timeline4 .timeline:last-child {
        margin: 0!important
    }
    .main-timeline4 .timeline-icon {
        right: auto;
        left: -14.5px
    }
    .main-timeline4 .year {
        border-radius: 50px 0 0 50px
    }
    .main-timeline4 .year:before {
        border-left: none;
        border-right: 35px solid transparent;
        left: auto;
        right: 0
    }
    .main-timeline4 .timeline-content {
        margin: 0 35px 0 45px
    }
} */

</style>