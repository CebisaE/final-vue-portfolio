<template>
<section id="contact" class="contact section-bg"> 
                <div class="container">
                    <div class="section-title">
          <h2>Contact</h2>
          <p>When you want to get in touch with me</p>
        </div>
                        <form @submit.prevent="submitform">
                                <label>Name:</label>
                                <input id="name" type="text"  required v-model="name" placeholder="your name">
                                <label>Email:</label>
                                <input id="email" type="email" required v-model="email" placeholder="your email">
                                <label>Contact:</label>
                                <input id="phone" type="cell" required v-model="contact" placeholder="your phone">
                                <label>Message:</label>
                                <input id="message" type="text" required v-model="message" placeholder="your message">
                            <div class=submit>
                                <button>submit</button>
                            </div>
                </form>
                    </div>
                
</section>

</template>

<script>
export default {
    data() {
        return{
            name: "",
            email:"",
            contact:"",
            message:"",
        }
    },
    methods: {
    submitform(){
        console.log('this.email,this.name,this.contact,this.message');
        fetch('https://emihle-portfolio-backend.herokuapp.com/contact', {
    method: 'POST',
    body: JSON.stringify({
    name: this.name,
    email: this.email,
    contact: this.contact,
    message: this.message,
}),
    headers: {
    'Content-type': 'application/json; charset=UTF-8',
    },
})
    .then((response) => response.json())
    .then((json) => console.log(json))
    .catch((e) => console.log(e))
    },



    },
    name: 'Contact',
    components: {
    }
}
</script>

<style scoped>
form{
    max-width:320px;
    margin:20px auto;
    text-align:left; 
    padding: 10px;
    border-radius: 10px;
}
label{
    color: #aaa;
    display: inline-block;
    margin:25px 0 15px;
    font-size:0.6em;
    text-transform: uppercase;
    letter-spacing:1px;
    font-weight: bold;
}
input{
    display: block;
    padding: 6px 2px;
    width: 100%;
    box-sizing: border-box;
    border: none;
    border-bottom: 1px solid #ddd;
    color: #555;
}
button{
    background: #173b6c;
    border:0;
    padding: 10px 20px;
    margin-top: 20px;
    color: white;
    border-radius: 20px;
    cursor: pointer;
}
button:hover {
    opacity: 0.8;
}
.submit{
    text-align: center;
}
.container{
    /* background: #f5f8fd; */
    overflow: hidden;
    padding:5em;
}

</style>