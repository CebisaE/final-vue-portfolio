<template>
<section>
    <h1 class="testihead">Below Are My Projects</h1>
<div  class="project-container">
<div v-for="project of projects" :key="project.id" class="projects">    
<div class="card" style="width: 18rem;">
    <img :src="project.img_url" class="card-img-top" alt="...">
<div class="card-body">
    <h2>{{project.title}}</h2>
</div>
<ul class="list-group list-group-flush">
    <li class="list-group-item">{{project.html}}</li>
    <li class="list-group-item">{{project.css}}</li>
    <li class="list-group-item">{{project.javascript}}</li>
</ul>
<div class="card-body">
    <a :href='project.github' class="card-link" target="_blank">github</a>
    <a :href='project.netlify' class="card-link" target="_blank">netlify</a>
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
    font-size: 2rem;
}
</style>