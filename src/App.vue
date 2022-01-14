<template>
  <img alt="Vue logo" src="./assets/logo.jpg" width="100">
  <sign-up/>
</template>

<script>
import SignUp from './components/signUp.vue'
export default {
  name: 'App',
  components:{
    SignUp
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
