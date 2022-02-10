<template>
  <img alt="Vue logo" src="./assets/logo.jpg">
  <p>Comprueba si puedes conducir</p>
  <check-age/>
</template>

<script>
import CheckAge from './components/CheckAge.vue'


export default {
  name: 'App',
  components: {
    CheckAge
    
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
