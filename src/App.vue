<template>
  <div id="app">
    <Header></Header>
    <Hero></Hero>
    <OnlineMarketing></OnlineMarketing>
    <TipsTricks></TipsTricks>
    <Features></Features>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Hero from "./components/Hero.vue";
import OnlineMarketing from "./components/OnlineMarketing.vue";
import TipsTricks from "./components/TipsTricks.vue";
import Features from "./components/Features.vue";

export default {
  name: "App",
  components: {
    Header,
    Hero,
    OnlineMarketing,
    TipsTricks,
    Features,
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
  p {
    color: #8e989f;
  }
  .btn {
    background-color: #377dff;
    &:hover {
      background-color: black;
      border-color: black;
    }
  }
}

.online-marketing {
  img {
    width: 80%;
  }
  p {
    color: #8e989f;
  }
  ul {
    list-style: none;
    margin-top: 1rem;
    padding-left: 0;
    margin-bottom: 0;
    li {
      padding-bottom: 0.5rem;
      i {
        color: #377dff;
        padding-right: 2rem;
      }
      a {
        text-decoration: none;
        color: black;
        &:hover {
          color: #377dff;
        }
      }
    }
  }
}

.tips-tricks {
  .d-flex {
    img {
      width: 30%;
      height: 30%;
      padding: 1rem;
    }
  }
  .evidence-box {
    border: 1px solid #00000014;
    box-shadow: 10px 20px 20px #00000014;
    h4 {
      color: #377dff;
    }
  }
  img {
    width: 100%;
  }
  p {
    color: #8e989f;
  }
}

.features {
  #circle-img {
    position: absolute;
    left: -25%;
    z-index: -1;
  }
  .btn {
    background-color: #377dff;
    &:hover {
      background-color: black;
      border-color: black;
    }
  }
  p {
    color: #8e989f;
  }
  .box {
    box-shadow: 0px 0px 30px 30px #00000014;
    margin-left: 0.5rem;
    margin-right: 0.5rem;
    margin-bottom: 2rem;
    width: calc((100% / 4) - 1rem);
    cursor: pointer;
    &:hover {
      color: white;
      background-color: #6cdac1 !important;
      box-shadow: none;
      transition: 0.3s;
    }
  }
}
</style>
