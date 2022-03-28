<template>
<section id="testimonials" class="testimonials">
   <div class="section-title">
          <h2>Testimonials</h2>
          <p>What my collegues and lectures think of me</p>
        </div>
    <div class="testimonial-container">
<div v-for="testimonial of testimonials" :key="testimonial.id" class="testimonial">  
      <div class="border">
            <img :src="testimonial.img_link" class="img-fluid" alt="image">
            <h4>{{testimonial.name}}</h4>
            <h6>{{testimonial.title}}</h6>
            <p>{{testimonial.text}}</p>
            <p>{{testimonial.email}}</p>
          </div>
        
  </div>  
    </div>
</section>
</template>

<script>
export default {
    data() {
      return {
        testimonials: []
      }
    },
mounted(){
    fetch('https://emihle-portfolio-backend.herokuapp.com/testimonials')
    .then(res => res.json())
    .then(data => {
      this.testimonials=data
      console.log(testimonials);
    })
    .catch(err => console.log(err.message))
},
  name: 'testimonials',
  components: {
  
  }
}
</script>

<style scoped>
.border p{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    overflow: hidden;
    font-size: 1rem;
}

.testimonial-container{
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap:30px;
  padding:86px;
}

.testimonial{
    display: flex;
    flex-wrap: wrap;
    flex-direction: row;
    gap: 15px;
    justify-content: center;
    width: 600px;
}
.border {
    font-family: sans-serif;
    font-size: 20px;
    font-weight: 700;
    color: black;
    border: 2px solid;
    padding: 20px;
    text-align: center;
    margin-bottom: 150px;
    min-width: 250px;
}
.border img {
    border-radius: 50%;
    height: 200px;
    width: 200px;
    object-fit: cover;
    margin-top: -125px;
    border: 2px solid;
}
.heading{
    padding-bottom: 129px;
    
}
.heading h1 {
    border-bottom: solid 4px black;
    margin: -0.512em auto;
    line-height: 1.2;
}
.border h4{
    font-size: 2.5rem;
    overflow: none;
}
.border h6{
    font-size: 1.5rem;
}
.email h6{
  font-size: 1rem;
}
</style>