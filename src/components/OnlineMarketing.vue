<template>
  <div class="online-marketing container my-5 py-5">
    <div class="row mt-5">
      <div class="col-4" v-for="(element, i) in marketingData" :key="i">
        <div class="d-flex">
          <div><img :src="element.src" :alt="element.title" /></div>
          <div class="d-flex flex-column">
            <h4>{{ element.title }}</h4>
            <p>
              {{ element.text }}
            </p>
            <ul>
              <li v-for="(element, i) in marketingLinks" :key="i">
                <i class="fa fa-check" aria-hidden="true"></i>
                <a :href="element.href">{{ element.txt }}</a>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "OnlineMarketing",
  data() {
    return {
      marketingData: [
        {
          src: require("../assets/img/24.png"),
          title: "Online Marketing",
          text: "It is a long established fact that a reader will be distracted.",
        },
        {
          src: require("../assets/img/24.png"),
          title: "Online Marketing",
          text: "It is a long established fact that a reader will be distracted.",
        },
        {
          src: require("../assets/img/24.png"),
          title: "Online Marketing",
          text: "It is a long established fact that a reader will be distracted.",
        },
      ],
      marketingLinks: [
        {
          txt: "SEO",
          href: "seo",
        },
        {
          txt: "SEM",
          href: "sem",
        },
        {
          txt: "Website Strategy",
          href: "website-strategy",
        },
        {
          txt: "Social managment",
          href: "social-managment",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
.online-marketing {
  img {
    width: 80%;
    cursor: pointer;
    transition: transform 0.3s;
    &:hover {
      transform: scale(1.5);
    }
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
</style>
