<template>
<!-- ======= Hero Section ======= -->
  <section id="hero" class="d-flex flex-column justify-content-center align-items-center">
    <div class="hero-container" data-aos="fade-in">
      <h1>Emihle Cebisa</h1>
      <p>WEB DEVELOPER / UI/UX DESIGNER</p>
    </div>
  </section><!-- End Hero -->
</template>

<script>
export default {
  name: "Home",
  
} 

</script>
<style scoped>
#hero {
  width: 183vh;
  height: 100vh;
  background: url("https://images.unsplash.com/photo-1555066931-4365d14bab8c?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1170&q=80") top center;
  background-size: cover;
}
#hero:before {
  position: absolute;
  bottom: 0;
  top: 0;
  left: 0;
  right: 0;
  z-index: 1;
}
.hero-container{
justify-content: center !important;

}
#hero .hero-container {
  position: relative;
  z-index: 2;
  min-width: 300px;
  
}
#hero h1 {
  font-size: 20vh;
  font-weight: 600;
  color: #fff;
  padding-bottom: 9px;
}
#hero p {
  padding-top:30px;
  color: #fff;
  margin-bottom: 50px;
  font-weight: 600;
  font-size: 5vh;
  font-family: "Poppins", sans-serif;
}

@media (max-width: 768px) {
  #hero h1 {
    font-size: 50px;
    line-height: 36px;
    padding: 5px;
  }
  #hero p {
    font-size: 18px;
    line-height: 24px;
    padding: 5px;
  }
}
* {
  box-sizing: border-box;
}

@keyframes openclose {
  0% {
    top: 0.2rem;
    width: 0;
  }
  5% {
    width: 0;
  }
  15% {
    width: 230px;
  }
  30% {
    top: 0.2rem;
    width: 230px;
  }
  33% {
    top: 0.2rem;
    width: 0;
  }
  35% {
    top: 0.2rem;
    width: 0;
  }
  38% {
    top: -4.5rem;
    
  }
  48% {
    top: -4.5rem;
    width: 190px;
  }
  62% {
    top: -4.5rem;
    width: 190px;
  }
  66% {
    top: -4.5rem;
    width: 0;
    text-indent: 0;
  }
  71% {
    top: -9rem;
    width: 0;
    text-indent: 5px;
  }
  86% {
    top: -9rem;
    width: 285px;
  }
  95% {
    top: -9rem;
    width: 285px;
  }
  98% {
    top: -9rem;
    width: 0;
    text-indent: 5px;
  }
  100% {
    top: 0;
    width: 0;
    text-indent: 0;
  }
}
</style>