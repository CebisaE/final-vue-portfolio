<template>
<section id="projects" class="project section-bg">

        <div class="section-title">
          <h2>Projects</h2>
          <p>Projects i've done since i joined Lifechoices</p>
        </div>

<div class="container my-5">
  <div v-for="project of projects" :key="project.id" class="card">
    <div class="imgBx">
      <img :src="project.img_url">
    </div>
    <div class="contentBx">
      <h2>{{project.title}}</h2>
      <!-- <a :href='project.github' class="card-link" target="_blank">github</a> -->
      <a :href='project.netlify' class="card-link" target="_blank">netlify</a>
    </div>
  </div>
</div>
</section>
</template>

<script>
export default {
    data() {
      return {
        projects: []
      }
    },
mounted(){
    fetch('https://emihle-portfolio-backend.herokuapp.com/projects')
    .then(res => res.json())
    .then(data => {
      this.projects=data
      console.log(projects);
    })
    .catch(err => console.log(err.message))
},
  name: 'Projects',
  components: {
  
  }
}
</script>

<style scoped>
.container{
  position: relative;
  display: flex;
  flex-direction: row;
  flex-wrap:wrap;
  justify-content: space-evenly;
  padding:3rem;
}

.container .card{
  position: relative;
  width: 320px;
  height: 450px;
  background: #fff;
  border-radius: 20px;
  overflow: hidden;
  margin-top: 50px;
}

.container .card:before{
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background:  #149ddd;;
  clip-path: circle(150px at 80% 20%);
  transition: 0.5s ease-in-out;
}

.container .card:hover:before{
  clip-path: circle(300px at 80% -20%);
}

.container .card:after{
  content: 'Work';
  position: absolute;
  top: 30%;
  left: -20%;
  font-size: 9em;
  font-weight: 800;
  font-style: italic;
  color:#149ddd;
}

.container .card .imgBx{
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  z-index: 10000;
  width: 100%;
  height: 220px;
  transition: 0.5s;
}

.container .card:hover .imgBx{
  top: 0%;
  transform: translateY(0%);
    
}

.container .card .imgBx img{
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%) rotate(-25deg);
  width: 270px;
}

.container .card .contentBx{
  position: absolute;
  bottom: 0;
  width: 100%;
  height: 100px;
  text-align: center;
  transition: 1s;
  z-index: 10;
}

.container .card:hover .contentBx{
  height: 210px;
}

.container .card .contentBx h2{
  position: relative;
  font-weight: 600;
  letter-spacing: 1px;
  color: #111;
  margin: 0;
}

.container .card .contentBx .size, .container .card .contentBx .color {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 8px 20px;
  transition: 0.5s;opacity: 0;
  visibility: hidden;
  padding-top: 0;
  padding-bottom: 0;
}

.container .card:hover .contentBx .size{
  opacity: 1;
  visibility: visible;
  transition-delay: 0.5s;
}

.container .card:hover .contentBx .color{
  opacity: 1;
  visibility: visible;
  transition-delay: 0.6s;
}

.container .card .contentBx .size h3, .container .card .contentBx .color h3{
  color: #111;
  font-weight: 300;
  font-size: 14px;
  text-transform: uppercase;
  letter-spacing: 2px;
  margin-right: 10px;
}

.container .card .contentBx .size span{
  width: 26px;
  height: 26px;
  text-align: center;
  line-height: 26px;
  font-size: 14px;
  display: inline-block;
  color: #fff;
  background: #fff;
  margin: 0 5px;
  transition: 0.5s;
  color: #fff;
  border-radius: 4px;
  cursor: pointer;
}

.container .card .contentBx .size span:hover{
  background:  #149ddd;;
}

.container .card .contentBx .color span{
  width: 20px;
  height: 20px;
  background:  #149ddd;;
  border-radius: 50%;
  margin: 0 5px;
  cursor: pointer;
}

.container .card .contentBx .color span:nth-child(2){
  background:  #149ddd;;
}

.container .card .contentBx .color span:nth-child(3){
  background: #03a9f4;
}

.container .card .contentBx .color span:nth-child(4){
  background: #111;
}

.container .card .contentBx a{
  display: inline-block;
  padding: 10px 20px;
  background: #111;
  border-radius: 4px;
  margin-top: 10px;
  text-decoration: none;
  font-weight: 600;
  color: #fff;
  opacity: 0;
  transform: translateY(50px);
  transition: 0.5s;
  margin-top: 0;
}

.container .card:hover .contentBx a{
  opacity: 1;
  transform: translateY(0px);
  transition-delay: 0.75s;
  
}

</style>