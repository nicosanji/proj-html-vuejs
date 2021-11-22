<template>
  <div id="app">
    <Header></Header>
    <Hero></Hero>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Hero from "./components/Hero.vue";

export default {
  name: "App",
  components: {
    Header,
    Hero,
  },
};
</script>

<style lang="scss">
@import "~bootstrap/scss/bootstrap";
@import "~font-awesome/css/font-awesome.min.css";

header {
  img {
    width: 5%;
    height: 5%;
    margin-right: auto;
  }
  ul {
    list-style: none;
    padding-left: 0;
    margin-bottom: 0;
    li {
      display: inline;
      a {
        text-decoration: none;
        color: black;
        font-weight: 500;
        &:hover {
          color: #377dff;
        }
      }
    }
    .active {
      color: #377dff;
      padding-bottom: 15px;
      border-bottom: 2px solid #377dff;
    }
  }
  p {
    margin-bottom: 0;
    cursor: pointer;
    &:hover {
      color: #377dff;
    }
    span {
      background-color: #377dff;
      color: white;
      font-weight: 500;
      right: 6px;
      bottom: 8px;
      height: 18px;
      width: 18px;
      font-size: 10px;
      line-height: 18px;
      text-align: center;
      border-radius: 50%;
      z-index: -1;
    }
  }
  .btn {
    background-color: #377dff;
    &:hover {
      background-color: black;
      border-color: black;
    }
  }
}

.my-hero {
  background-color: #f2f7ff;
  img {
    width: 90%;
    top: 20px;
    right: 0;
  }
  .btn {
    background-color: #377dff;
    &:hover {
      background-color: black;
      border-color: black;
    }
  }
}
</style>
