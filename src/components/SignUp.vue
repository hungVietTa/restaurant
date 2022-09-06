<template>
    <img src="../assets/logo.png" class="logo" alt="">
     <h1>Sign Up</h1>
     <div class="register">
        <input type="text" v-model="name" placeholder="Enter Name">
        <input type="text" v-model="email" placeholder="Enter Email">
        <input type="text" v-model="password" placeholder="Enter Password">
        <button @click="signUp">Sign Up</button>
     </div>
</template>
<script>
import axios from 'axios'
export default {
  name: 'SignUp',
  data() {
    return {
        name:"",
        email:'',
        password:''
    }
  },
  methods:{
    signUp() {
        console.warn("signup",this.name,this.email,this.password)
    }
  }
}
</script>
<style>
    .logo {
        width: 100px;
    }
    .register input {
        width:300px;
        height: 40px;
        padding-left: 20px;
        display: block;
        margin-bottom: 30px;
        margin-right: auto;
        margin-left: auto;
    }
    .register button {
        width: 320px;
        height: 40px;
        border: 1px solid skyblue;
        background-color: skyblue;
        color: white;
        cursor: pointer;
    }
</style>