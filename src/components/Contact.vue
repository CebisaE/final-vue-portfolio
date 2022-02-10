<template>
<section id="contact" style="height:100vh">
                <div class="container">
                    <div>
                        <span class="touch">Get In Touch</span>
                        <h3 class="touches">Connect With Me Below</h3>
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
        fetch('http://localhost:5000/contact', {
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
    max-width:420px;
    margin:30px auto;
    background: white;
    text-align:left; 
    padding: 40px;
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
    padding: 10px 6px;
    width: 100%;
    box-sizing: border-box;
    border: none;
    border-bottom: 1px solid #ddd;
    color: #555;
}
button{
    background: #ea4343;
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

.touch{
    font-family: sans-serif;
    font-size: 70px;
    color: #fff;
    font-weight: 700;
    letter-spacing: -.2px;
    display: inline-block;
    margin-bottom: 5px;
}
.touches{
    font-family: sans-serif;
    font-size: 30px;
    color: #fff;
    font-weight: 700;
    margin-bottom: 1px;
    padding: 16px;
}

</style>