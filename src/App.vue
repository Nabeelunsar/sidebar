<template>
  <div class="main-page">
    <header />
    <div class="main">
      <sidebar />
      <c />
    </div>
  </div>
</template>

<script>
import header from "./components/header.vue";
import sidebar from "./components/sidebar.vue";
import c from "./components/c.vue";
export default {
  name: "App",
  components: {
    header,
    sidebar,
    c,
  },
};
</script>
<style>
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

.main {
  display: flex
}
</style>
