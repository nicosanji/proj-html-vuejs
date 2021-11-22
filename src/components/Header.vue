<template>
  <header>
    <div class="container d-flex align-items-center">
      <img src="../assets/img/logo-2.png" alt="logo-2" class="py-2" />
      <ul>
        <li v-for="(element, i) in headerLinks" :key="i" class="px-3">
          <a
            @click.prevent="currentIndex = i"
            :class="i === currentIndex ? 'active' : ''"
            href="element.href"
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
          href: "home",
        },
        {
          txt: "About us",
          href: "about-us",
        },
        {
          txt: "Feature",
          href: "feature",
        },
        {
          txt: "Testimonials",
          href: "testimonials",
        },
        {
          txt: "Contact US",
          href: "contact-us",
        },
      ],
    };
  },
};
</script>

<style></style>
