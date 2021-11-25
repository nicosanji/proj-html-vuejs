<template>
  <header>
    <div class="container d-flex align-items-center" id="home">
      <img src="../assets/img/logo-2.png" alt="logo-2" class="py-2" />
      <ul>
        <li v-for="(element, i) in headerLinks" :key="i" class="px-3">
          <a
            @click="currentIndex = i"
            :class="i === currentIndex ? 'active' : ''"
            :href="element.href"
            >{{ element.txt }}</a
          >
        </li>
      </ul>
      <p class="ps-5 pe-3"><i class="fa fa-search" aria-hidden="true"></i></p>
      <p class="px-3 position-relative">
        <i class="fa fa-shopping-cart" aria-hidden="true"></i>
        <span class="position-absolute">0</span>
      </p>
      <div>
        <button type="button" class="btn text-white px-3 py-2 ms-5">
          Get Started
        </button>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      currentIndex: 0,
      headerLinks: [
        {
          txt: "Home",
          href: "#home",
        },
        {
          txt: "About us",
          href: "#about-us",
        },
        {
          txt: "Feature",
          href: "#feature",
        },
        {
          txt: "Testimonials",
          href: "#testimonials",
        },
        {
          txt: "Contact US",
          href: "#contact-us",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "@/assets/styles/variables.scss";

header {
  img {
    width: 5%;
    height: 5%;
    margin-right: auto;
    cursor: pointer;
    transition: transform 1s;
    &:hover {
      transform: rotate(360deg);
    }
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
          color: $my-blue;
        }
      }
    }
    .active {
      color: $my-blue;
      padding-bottom: 15px;
      border-bottom: 2px solid $my-blue;
    }
  }
  p {
    margin-bottom: 0;
    cursor: pointer;
    &:hover {
      color: $my-blue;
    }
    span {
      background-color: $my-blue;
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
    background-color: $my-blue;
    &:hover {
      background-color: black;
      border-color: black;
    }
  }
}
</style>
