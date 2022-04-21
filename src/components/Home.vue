<template>
 <section id="hero" class="d-flex flex-column justify-content-center align-items-center">
    <div class="hero-container" data-aos="fade-in">
      <h1>Emihle Cebisa</h1>
      <h2>
  <span>Aspiring</span>
  <div class="message">
    <div class="word1">UI/UX</div>
    <div class="word3">Web Dev</div>
  </div>
</h2>
    </div>
  </section>
</template>

<script>
export default {
  name: "Home",
  components: {
  },
  
} 

</script>
<style scoped>
#hero {
  width: 100%;
  height: 100vh;
  background: url("https://i.postimg.cc/90rgvx21/photo-1498050108023-c5249f4df085.jpg") top center;
  background-size: cover;
}
#hero:before {
  content: "";
  background: rgba(5, 13, 24, 0.3);
  position: absolute;
  bottom: 0;
  top: 0;
  left: 0;
  right: 0;
  z-index: 1;
  height: 100vh;
width: 110em;
}
.hero-container{
align-self: center;

}
#hero .hero-container {
  position: relative;
  z-index: 2;
  min-width: 300px;
  
}
#hero h1 {
  font-size: 64px;
  font-weight: 700;
  line-height: 56px;
  color: #fff;
}

@media (max-width: 768px) {
  #hero h1 {
    font-size: 28px;
    line-height: 36px;
  }
  #hero h2 {
    font-size: 18px;
    line-height: 24px;
    /* margin-bottom: 30px; */
  }
}
* {
  box-sizing: border-box;
}


body {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 100vh;
  width: 100vw;
}
h2 {
  color: #fff;
  font-family: tahoma;
  font-size: 3rem;
  font-weight: 100;
  line-height: 1.5;
  text-transform: uppercase;
  white-space: nowrap;
  overflow: hidden;
  position: relative;
  width: 550px;
}

h2 span {
  font-size: 40px;
  font-weight: 900;
  margin-left: -185px;
}

.message {
  color: #fff;
  display: block;
  font-weight: 900;
  /* overflow: hidden; */
  position: absolute;
  padding-left: 1.4rem;
  top: 0.rem;
  left: 270px;
  animation: openclose 8s ease-in-out infinite;
}

.word1,.word3 {
  font-family: tahoma;
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