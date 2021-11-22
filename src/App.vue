<template>
  <div id="app">
    <Header></Header>
  </div>
</template>

<script>
import Header from "./components/Header.vue";

export default {
  name: "App",
  components: {
    Header,
  },
};
</script>

<style lang="scss">
@import "~bootstrap/scss/bootstrap";
@import "~font-awesome/css/font-awesome.min.css";
</style>
