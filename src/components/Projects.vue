<template>
<section>
    <h1 class="testihead">Below Are My Projects</h1>
<div  class="project-container">
<div v-for="project of projects" :key="project.id" class="projects">    
<div class="card mb-3" style="max-width: 540px;">
  <div class="row g-0">
    <div class="col-md-4">
      <img :src="project.img_url" class="img-fluid rounded-start" alt="...">
    </div>
    <div class="col-md-8">
      <div class="card-body">
        <h5 class="card-title">{{project.title}}</h5>
        <p>{{project.details}}</p>
        <ul style="list-style: none">
        <li>{{project.html}}</li>
        <li>{{project.css}}</li>
        <li>{{project.javascript}}</li>
        </ul>
        <a :href='project.github' class="card-link" target="_blank">github</a>
        <a :href='project.netlify' class="card-link" target="_blank">netlify</a>
      </div>
    </div>
  </div>
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
.img-fluid{
height: 250px;
object-fit: cover;
width: 300px;
}
.project-container {
    padding: 161px;
    margin: 117px;
    margin-top:-111px;
    
    display: grid;
    flex-direction: column;
    grid-gap: 1rem;
    justify-content: space-evenly;
    flex-wrap: wrap;
    grid-template-columns: repeat(3 ,1fr);
}
.labels{
    font-family: sans-serif;
    font-size: 20px;
    font-weight: 700;
    color: black;
}
.testihead{
    font-weight: 700;
    color: white;
    font-size: 7rem;
}
</style>