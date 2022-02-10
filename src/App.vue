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
  background-color: #2c3e50;
}
</style>
