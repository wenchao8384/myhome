<template>
  <div id="app">
    <Header msg="Welcome to Your Vue.js App"/>
    <NavBar/>
  </div>
</template>

<script>
import Header from './components/header.vue'
import NavBar from './components/navBar.vue'

export default {
  name: 'App',
  components: {
    Header,
    NavBar
  }
}
</script>

<style>
#app {
  
}
</style>
