<template>
  <footer class="bg-dark text-center text-white footer">
    <!-- Grid container -->
    <div class="container p-4 pb-0">
      <!-- Section: Social media -->
      <section class="mb-4">
        <!-- Linkedin -->
        <a
          class="btn btn-outline-light btn-floating m-1"
          href="https://www.linkedin.com/in/emihle-cebisa-60292b223" 
          role="button"
          target="_blank"
          ><i class="fab fa-linkedin-in"></i
        ></a>

        <!-- Github -->
        <a
          class="btn btn-outline-light btn-floating m-1"
          href="https://github.com/CebisaE/" 
          role="button"
          target="_blank"
          ><i class="fab fa-github"></i
        ></a>

        <!-- Codepen -->
        <a
          class="btn btn-outline-light btn-floating m-1"
          href="https://codepen.io/cebisae"
          role="button"
          target="_blank"
          ><i class="fab fa-codepen"></i
        ></a>
      </section>
      <!-- Section: Social media -->
    </div>
    <!-- Grid container -->

    <!-- Copyright -->
    <div class="text-center p-3" style="background-color: rgba(0, 0, 0, 0.2)">
      © 2022 Copyright:
      <a class="text-white" href="https://mdbootstrap.com/"
        >Emihle Cebisa</a
      >
    </div>
    <!-- Copyright -->
  </footer>

</template>
<script>
  import { MDBFooter } from 'mdb-vue-ui-kit';
  export default {
    components: {
      MDBFooter
    },
  };
</script>