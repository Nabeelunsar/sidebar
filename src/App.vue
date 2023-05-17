


<template>
  <div class="main-page">
    <header1 />
    <div class="main">
      <bodymain />
      <sidebar />
    </div>
  </div>
</template>

<script>
import header1 from './components/header1.vue';
import sidebar from './components/sidebar.vue';
import bodymain from './components/bodymain.vue';

export default {
  name: 'App',
  components: {
    header1,
    sidebar,
    bodymain,
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
