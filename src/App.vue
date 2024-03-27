<template>
  <div id="app">
    <Header/>
    <img alt="Vue logo" src="./assets/imagenProyecto.jpg">
    <AppForm/>
  </div>
</template>

<script>
import Header from './components/AppHeader.vue'
import AppForm from './components/AppForm.vue'


export default {
  name: 'App',
  components: {
    Header,
    AppForm,

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
