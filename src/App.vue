<template>
  <div>
    <login-page/>
  </div>
</template>

<script>
import LoginPage from './components/LoginPage/LoginPage.vue'

export default {
  components: { LoginPage },
  name: 'App',
  data(){
    return{
      title: 'Home'
    }
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
