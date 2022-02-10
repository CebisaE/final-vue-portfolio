<template>
<section id="nav">
<nav class="navbar navbar-dark bg-dark">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">E.Cebisa</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarText" aria-controls="navbarText" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarText">
      <ul class="navbar-nav me-auto mb-2 mb-lg-0">
        <li class="nav-item">
            <a class="nav-link" href="#home">Contacts</a>
          </li>
         <li class="nav-item">
            <a class="nav-link" href="#about">Contacts</a>
          </li>
         <li class="nav-item">
            <a class="nav-link" href="#resume">Contacts</a>
          </li>
           <li class="nav-item">
            <a class="nav-link" href="#projects">Contacts</a>
          </li>
        <li class="nav-item">
            <a class="nav-link" href="#testimonals">Contacts</a>
          </li>
        <li class="nav-item">
            <a class="nav-link" href="#contact">Contacts</a>
          </li>
      </ul>
    </div>
  </div>
</nav>
</section>
</template>

<script>
export default {

}
</script>

<style>


#nav a {
font-weight: bold;
/* color: black; */
text-decoration: none;
padding: 10px;
border-radius: 4px;
}

.nav-item :hover{
color: red;
transition: 0.3s;
}
div#navbarNavDropdown {
    justify-content: end;
}
</style>