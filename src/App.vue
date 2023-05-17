<template>
  <header1/>
  <bodymain/>
  <sidebar/>
</template>

<script>
import header1 from './components/header.vue'
import sidebar from './components/sidebar.vue'
import bodymain from './components/header.vue'

export default {
  name: 'App',
  components: {
    header1,
    sidebar,
    bodymain
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
