<template>
  <footer class="border-top py-5">
    <div class="container">
      <div class="row justify-content-evenly align-items-evenly">
        <div class="col-3">
          <img src="../assets/img/35.png" alt="logo-png" />
          <p class="pt-2 pb-4">
            It is a long established fact that a reader will be distracted by
            the readable content.
          </p>
          <p>Copyright @ 2018 <span>SofBox</span></p>
        </div>
        <div class="col-2">
          <h5>Menu</h5>
          <ul>
            <li v-for="(element, i) in menuLinks" :key="i">
              <a :href="element.href">{{ element.txt }}</a>
            </li>
          </ul>
        </div>
        <div class="col-2">
          <h5>About Us</h5>
          <ul>
            <li v-for="(element, i) in aboutLinks" :key="i">
              <a :href="element.href">{{ element.txt }}</a>
            </li>
          </ul>
        </div>
        <div class="col-2">
          <h5>Quick Links</h5>
          <ul>
            <li v-for="(element, i) in quickLinks" :key="i">
              <a :href="element.href">{{ element.txt }}</a>
            </li>
          </ul>
        </div>
      </div>
    </div>
    <div class="container-fluid d-flex flex-row-reverse">
      <h1>
        <a href="#top"
          ><i class="fa fa-chevron-circle-up" aria-hidden="true"></i
        ></a>
      </h1>
    </div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
  data() {
    return {
      menuLinks: [
        {
          txt: "About us",
          href: "about-us",
        },
        {
          txt: "Theme",
          href: "theme",
        },
        {
          txt: "Features",
          href: "features",
        },
        {
          txt: "Pricing",
          href: "pricing",
        },
        {
          txt: "Blog",
          href: "blog",
        },
      ],
      aboutLinks: [
        {
          txt: "About Sofbox",
          href: "about-sofbox",
        },
        {
          txt: "Roadmap",
          href: "roadmap",
        },
        {
          txt: "How it Work",
          href: "how-it-work",
        },
        {
          txt: "Team",
          href: "team",
        },
        {
          txt: "News",
          href: "news",
        },
      ],
      quickLinks: [
        {
          txt: "About us",
          href: "about-us",
        },
        {
          txt: "Theme",
          href: "theme",
        },
        {
          txt: "Features",
          href: "features",
        },
        {
          txt: "Pricing",
          href: "pricing",
        },
        {
          txt: "Blog",
          href: "blog",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
footer {
  p {
    color: #8e989f;
  }
  span {
    color: #377dff;
  }
  ul {
    list-style: none;
    padding-left: 0;
    margin-bottom: 0;
    li {
      padding: 0.25rem 0;
      a {
        text-decoration: none;
        color: #8e989f;
        &:hover {
          color: #377dff;
        }
      }
    }
  }
  h1 {
    a {
      text-decoration: none;
      color: #8e989f;
      &:hover {
        color: #377dff;
      }
    }
  }
}
</style>
