<template>
  <div class="my-hero container-fluid pb-5 mt-2 mb-5">
    <div class="row">
      <div class="col-5 px-5 py-5">
        <h1 class="mb-0 py-5">The biggest platform for your growth.</h1>
        <p class="mb-0">
          Thare are many variations of passage of Lorem Ipsum available, but the
          majority have suffered alteration in some form
        </p>
        <button class="btn text-white px-3 py-2 my-5">Read More</button>
      </div>
      <div class="col-7 position-relative">
        <img
          class="position-absolute"
          src="../assets/img/27-1.png"
          alt="hero-img"
        />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Hero",
};
</script>

<style lang="scss">
@import "@/assets/styles/variables.scss";

.my-hero {
  background-color: $my-lightblue;
  img {
    width: 90%;
    top: 20px;
    right: 0;
  }
  p {
    color: $my-gray;
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
