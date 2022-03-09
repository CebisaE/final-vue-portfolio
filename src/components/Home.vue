<template>
 <section id="hero" class="d-flex flex-column justify-content-center align-items-center">
    <div class="hero-container" data-aos="fade-in">
      <h1>Emihle Cebisa</h1>
    </div>
    <div class="typing-slider">
  <p class="type">Aspiring Fullstack Developer</p>
  <p class="type">Web Developer</p>
  <p class="type">Freelancer</p>
</div>
  </section>
</template>

<script>
export default {
  name: "Home",
  components: {
  }
}

</script>
<style>
#hero {
  width: 100%;
  height: 100vh;
  background: url("https://i.postimg.cc/ZnBdxDLH/rsz-1img-20220228-wa0028-min.jpg") top center;
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
}
#hero .hero-container {
  position: relative;
  z-index: 2;
  min-width: 300px;
}
#hero h1 {
  margin: 0 0 10px 0;
  font-size: 64px;
  font-weight: 700;
  line-height: 56px;
  color: #fff;
}
#hero p {
  color: #fff;
  margin-bottom: 50px;
  font-size: 26px;
  font-family: "Poppins", sans-serif;
}
#hero p span {
  color: #fff;
  padding-bottom: 4px;
  letter-spacing: 1px;
  border-bottom: 3px solid #149ddd;
}
@media (min-width: 1024px) {
  #hero {
    background-attachment: fixed;
  }
}
@media (max-width: 768px) {
  #hero h1 {
    font-size: 28px;
    line-height: 36px;
  }
  #hero h2 {
    font-size: 18px;
    line-height: 24px;
    margin-bottom: 30px;
  }
}
@keyframes cursor {
  from, to {
    border-color: transparent;
  }
  50% {
    border-color: black;
  }
}
@keyframes typing {
  from {
    width: 100%;
  }
  90%, to {
    width: 0;
  }
}
@keyframes slide {
  33.3333333333% {
    font-size: 3rem;
    letter-spacing: 3px;
  }
  to {
    font-size: 0;
    letter-spacing: 0;
  }
}
.type{
  color: white;
}
.typing-slider {
  font-family: Consolas, monospace;
  font-weight: bold;
  text-align: center;
  color: white !important;
  white-space: nowrap;
}

.typing-slider p {
  position: relative;
  display: inline;
  font-size: 0;
  color: #fff!important;
  text-transform: uppercase;
  letter-spacing: 0;
  animation: slide 15s step-start infinite;
}

.typing-slider p::after {
  content: "";
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  border-left: 3px solid black;
  animation: typing 5s infinite, cursor 1s infinite;
}

.typing-slider p:nth-child(1) {
  animation-delay: 0s;
}
.typing-slider p:nth-child(1)::after {
  animation-delay: 0s;
  animation-timing-function: steps(16), step-end;
}

.typing-slider p:nth-child(2) {
  animation-delay: 5s;
}
.typing-slider p:nth-child(2)::after {
  animation-delay: 5s;
  animation-timing-function: steps(23), step-end;
}

.typing-slider p:nth-child(3) {
  animation-delay: 10s;
}
.typing-slider p:nth-child(3)::after {
  animation-delay: 10s;
  animation-timing-function: steps(12), step-end;
}
</style>