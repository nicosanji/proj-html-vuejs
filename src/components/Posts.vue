<template>
  <div class="posts py-5">
    <div class="w-50 mx-auto">
      <h2 class="text-center">Latest Posts</h2>
      <p class="text-center mt-4">
        If you are planning on developing a product landing.
      </p>
    </div>
    <div class="container">
      <div class="row justify-content-evenly pt-5">
        <div class="col-4" v-for="(element, i) in postsData" :key="i">
          <div class="card w-100 p-2 position-relative">
            <div
              class="position-absolute bg-white rounded-1 px-2 py-1 ms-2 mt-2"
            >
              <p class="mb-0">{{ element.day }}</p>
            </div>
            <img :src="element.src" class="card-img-top" :alt="element.title" />
            <div class="card-body">
              <h5 class="card-title my-3">{{ element.title }}</h5>
              <p class="card-text pe-5">
                {{ element.text }}
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "PostsPlus",
  data() {
    return {
      postsData: [
        {
          src: require("../assets/img/19.jpg"),
          day: "November 28, 2019",
          title: "Life Lack Meaning",
          text: "It is a long established fact that a reader will be distracted by the readable.",
        },
        {
          src: require("../assets/img/18.jpg"),
          day: "November 28, 2019",
          title: "Life Lack Meaning",
          text: "It is a long established fact that a reader will be distracted by the readable.",
        },
        {
          src: require("../assets/img/17.jpg"),
          day: "November 28, 2019",
          title: "Life Lack Meaning",
          text: "It is a long established fact that a reader will be distracted by the readable.",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
.posts {
  .card {
    cursor: pointer;
    transition: transform 0.3s, box-shadow 0.3s;
    &:hover {
      transform: scale(1.1);
      box-shadow: 0px 0px 30px 30px #00000014;
    }
  }
  p {
    color: #8e989f;
  }
}
</style>
