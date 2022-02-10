<template>
<section id="home" class="emihle-section">
  <div class="container"></div>
<div class="myTitle">
    <h2 class="myTitle"><span >Hello, I'm <br> Emihle Cebisa</span><br>
                  Aspiring
          <span class="title">Fullstack Developer</span>
    </h2>

  </div>
<div id="carouselExampleIndicators" class="carousel slide" data-bs-ride="carousel" style="height:90vh">
  <div class="carousel-indicators">
    <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
    <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="1" aria-label="Slide 2"></button>
    <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="2" aria-label="Slide 3"></button>
  </div>
  <div class="carousel-inner">
    <div class="carousel-item active">
      <img src="https://images.unsplash.com/photo-1517694712202-14dd9538aa97?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8MTl8fGNvZGluZ3xlbnwwfHwwfHw%3D&auto=format&fit=crop&w=500&q=60" class="d-block w-100" alt="..." style="height:90vh">

    </div>
    <div class="carousel-item">
      <img src="https://images.unsplash.com/photo-1554306274-f23873d9a26c?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=870&q=80" class="d-block w-100" alt="..." style="height:90vh">
    </div>
    <div class="carousel-item">
      <img src="https://images.unsplash.com/photo-1484417894907-623942c8ee29?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1032&q=80" class="d-block w-100" alt="..." style="height:90vh">
    </div>
  </div>
  <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="prev">
    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Previous</span>
  </button>
  <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="next">
    <span class="carousel-control-next-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Next</span>
  </button>
</div>
</section>
</template>

<script>

export default {
  name: 'Home',
  components: {
  }
}

</script>
<style>
.myTitle {
  text-align: center;
  position: absolute;
  height:100vh;
  width: 100vw;
  display: flex;
  justify-content: center;
  flex-direction: column;
  color: red;
  z-index: 5;
  pointer-events: none;
  font-weight: 700;
  font-size: 5vw;
}
</style>