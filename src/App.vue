<template>
  <Navbar/>
  <Home/>
  <About/>
  <Resume/>
  <Projects/>
  <Testimonials/>
  <Contact/>
  <Footer/>
</template>

<script>
import Projects from './components/Projects.vue'
import Testimonials from './components/Testimonials.vue'
import Home from './components/Home.vue'
import About from './components/About.vue'
import Resume from './components/Resume.vue'
import Contact from './components/Contact.vue'
import Navbar from './components/Navbar.vue'
import Footer from './components/Footer.vue'
export default {
  name: 'App',
  components: {
    Navbar,
    Home,
    About,
    Resume,
    Projects,
    Testimonials,
    Contact,
    Footer
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  background-color: white;
}
/* sections style */
section {
  padding: 60px 0;
  overflow: hidden;
}

.section-bg {
  background: #f5f8fd;
}

.section-title {
  padding-bottom: 30px;
}
.section-title h2 {
  font-size: 32px;
  font-weight: bold;
  margin-bottom: 20px;
  padding-bottom: 20px;
  position: relative;
  color: #173b6c;
}
.section-title h2::after {
  content: "";
  position: absolute;
  display: block;
  width: 50px;
  height: 3px;
  background: #149ddd;
  bottom: 0;
  left: 0;
}
.section-title p {
  margin-bottom: 0;
}
</style>
