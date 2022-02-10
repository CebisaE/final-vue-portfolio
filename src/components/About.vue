<template>
<section class="about" style="padding:15px">
<div class="row-1">
<div class="image">
<img src="https://i.postimg.cc/DyfB3MMF/Emihle2-min.jpg" alt="">
</div>
<div class="content">
<h3>Hi my name is Emihle ,an aspiring developer that's ready to 
      learn new things to improve her skill</h3>
<p>My love for coding began a long time ago,
      just that I didn't have the opportunity to do coding
      A family friend introduced me to coding,
      when he told me to try out Lifechoices since he knew that
      I am interested in technology.</p>
<div class="box-container">
    <div class="box">
        <p> <span> gender : </span> Female </p>
        <p> <span> language : </span> english </p>
        <p> <span> work : </span> fullstack developer </p>
    </div>
    <div class="box">
        <p> <span>freelance : </span> available </p>
        <p> <span> phone : </span> 074 737 7043 </p>
        <p> <span> country : </span> South Africa </p>
    </div>
</div>
    <h3 class="skills">Skills
    </h3><br>
<MDBRow class="Skill" style="max-width: 740px">
          <MDBCol col="6" sm="4"
            ><img
              src="https://i.postimg.cc/3JQc9HfW/4691516-html5-icon.png"
              alt=""
              class="img-fluid rounded"
          /></MDBCol>
          <MDBCol col="6" sm="4"
            ><img
              src="https://i.postimg.cc/RhvPmB2d/8546808-bootstrap-icon.png"
              alt=""
              class="img-fluid rounded"
          /></MDBCol>
          <MDBCol col="6" sm="4"
            ><img
              src="https://i.postimg.cc/JhBYcKbN/7422531-css3-css-file-development-icon.png"
              alt=""
              class="img-fluid rounded"
          /></MDBCol>
          <MDBCol col="6" sm="4"
            ><img
              src="https://i.postimg.cc/nhRT8824/8674900-ic-fluent-javascript-regular-icon.png"
              alt=""
              class="img-fluid rounded"
          /></MDBCol>
          <MDBCol col="6" sm="4"
            ><img
              src="https://i.postimg.cc/053x9XVv/4691303-mysql-icon.png"
              alt=""
              class="img-fluid rounded"
          /></MDBCol>

          <div class="w-100 d-none d-md-block"></div>

          <MDBCol col="6" sm="4"
            ><img
              src="https://i.postimg.cc/rpd3ZqLt/4691448-dot-js-vue-icon.png"
              alt=""
              class="img-fluid rounded"
          /></MDBCol>
          <MDBCol col="6" sm="4"
            ><img
              src=" https://i.postimg.cc/Bnjm4N7r/8546865-git-alt-icon.png"
              alt=""
              class="img-fluid rounded"
          /></MDBCol>
          <MDBCol col="6" sm="4"
            ><img
              src="https://i.postimg.cc/X7GnB51d/Screenshot-from-2022-01-28-10-56-10-removebg-preview.png"
              alt=""
              class="img-fluid rounded"
          /></MDBCol>
          <MDBCol col="6" sm="4"
            ><img
              src="https://i.postimg.cc/G2g1H3kX/Screenshot-from-2022-01-28-10-58-18-removebg-preview.png"
              alt=""
              class="img-fluid rounded"
          /></MDBCol>
          <MDBCol col="6" sm="4"
            ><img
              src="https://i.postimg.cc/d109dkPX/Screenshot-from-2022-01-28-11-03-23-removebg-preview.png"
              alt=""
              class="img-fluid rounded"
          /></MDBCol>
        </MDBRow>
</div>
</div>
</section>
</template>

<script>
export default {
  name: 'About',
  components: {

  }
}
</script>

<style scoped>

.about .row-1{
display: flex;
flex-wrap: wrap;
gap:1.5rem;
padding-bottom: 2rem;
}
.about .row-1 .image{
flex:1 1 25rem;
}
.about .row-1 .image img{
height: 100%;
width:100%;
object-fit: cover;
border:1rem solid #fff;
border-radius: .5rem;
box-shadow: 0 .5rem 1rem rgba(0,0,0,.1);
}
.about .row-1 .content{
flex:1 1 50rem;
}

.about .row-1 .content h3{
color:#ea4343 ;
font-family: sans-serif;
    font-size: 2.3rem;
    font-weight: 700;
}
.about .row-1 .content p{
color:#fff;
font-size: 1.9rem;
padding:.5rem 0;
}
.about .row-1 .content .box-container{
display: flex;
flex-wrap: wrap;
gap:1.5rem;
padding: 5rem 0;
}
.about .row-1 .content .box-container .box{
flex:1 1 20rem;
}
.about .row-1 .content .box-container .box span{
color:var(--main-color); 
}
.skill{
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  gap: 40px;
  
}
.skills{
    font-family: sans-serif;
    font-size: 60px;
    font-weight: 700;
    color:#ea4343 ;
    letter-spacing: -.2px;
    display: inline-block;
    margin-bottom: 6px;
}
.img-fluid {
  height: 200px;
  border: 3px solid white;
  padding: 50px;
  margin: 1%;
  border-radius: 10px;
}
</style>