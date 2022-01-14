<template>
<h1>Sign Up</h1>
<div class="register">
  <input type="text" v-model="name" placeholder="Enter Name" />
  <input type="email" v-model="email" placeholder="Enter Email" />
  <input type="password" v-model="password" placeholder="Enter Password" />
  <button v-on:click="signUp">SignUp</button>
</div>
</template>
<script>
// import axios from 'axios'
export default{
  name: 'SignUp',
  data()
  {
    return{
      name:'',
      email:'',
      password:''
    }
  },
  methods:{
    // async
    signUp()
    {
      console.warn("signup",this.name,this.email,this.password)
      // let result = await axios.post("http://localhost:3000/user",{
      //   email:this.email,
      //   name:this.name,
      //   password:this.password
      // });

      // console.warn(result);
      // if(result.status=201){
      //   alert("Signed Up Successfully");
      // }
    }

  }
}
</script>

<style>
  .register input{
  width: 300px;
  height: 40px;
  padding-left: 20px;
  display: block;
  margin-bottom: 30px;
  margin-left: auto;
  margin-right: auto;
  border: 1px solid skyblue;
}

.register button{
  width: 320px;
  height: 40px;
  border: 1px solid rgb(27, 134, 153);
  background-color: rgb(27, 134, 153);
  cursor: pointer;
  color: white;
  text-decoration-thickness: 2px;
}
</style>