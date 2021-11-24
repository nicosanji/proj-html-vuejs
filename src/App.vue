<template>
  <div id="app">
    <Header></Header>
    <Hero></Hero>
    <OnlineMarketing></OnlineMarketing>
    <TipsTricks></TipsTricks>
    <Features></Features>
    <Testimonials></Testimonials>
    <Posts></Posts>
    <Contact></Contact>
    <Footer></Footer>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Hero from "./components/Hero.vue";
import OnlineMarketing from "./components/OnlineMarketing.vue";
import TipsTricks from "./components/TipsTricks.vue";
import Features from "./components/Features.vue";
import Testimonials from "./components/Testimonials.vue";
import Posts from "./components/Posts.vue";
import Contact from "./components/Contact.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    Hero,
    OnlineMarketing,
    TipsTricks,
    Features,
    Testimonials,
    Posts,
    Contact,
    Footer,
  },
};
</script>

<style lang="scss">
@import "~bootstrap/scss/bootstrap";
@import "~font-awesome/css/font-awesome.min.css";
</style>
