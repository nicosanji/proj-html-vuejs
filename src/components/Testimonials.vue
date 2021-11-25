<template>
  <div class="testimonials mb-5" id="testimonials">
    <img class="" src="../assets/img/15.png" alt="wave-img" />
    <div class="w-50 mx-auto mb-5">
      <h2 class="text-center">Our Testimonials</h2>
      <p class="text-center mt-4">
        If you are planning on developing a product landing app or website,<br />
        take a look at this beautiful-crafted
      </p>
    </div>
    <div class="container pt-5">
      <div class="row justify-content-evenly">
        <div
          class="col-5 d-flex flex-column align-items-center border py-2 px-4"
        >
          <img
            class="rounded-circle border border-4 border-white mb-5"
            src="../assets/img/26.jpeg"
            alt="test-w-img"
          />
          <h4 class="mb-3">Juila Aann <span>- COO Sofbox</span></h4>
          <p class="py-3">
            At ver eos et accusamus et iusto odio dignissimos <br />
            ducimus qui blanditiis praesentium vero eos et consectetur <br />
            accus adip adip.
          </p>
        </div>
        <div
          class="col-5 d-flex flex-column align-items-center border py-2 px-4"
        >
          <img
            class="rounded-circle border border-4 border-white mb-5"
            src="../assets/img/27.jpeg"
            alt="test-w-img"
          />
          <h4 class="mb-3">Mac Znder <span>- Manager Sofbox</span></h4>
          <p class="py-3">
            At ver eos et accusamus et iusto odio dignissimos <br />
            ducimus qui blanditiis praesentium vero eos et consectetur <br />
            accus adip adip.
          </p>
        </div>
      </div>
      <div class="text-center my-4 pt-4">
        <h5 tabindex="0">
          <i class="fa fa-circle" aria-hidden="true"></i>
        </h5>
        <h5 tabindex="0">
          <i class="fa fa-circle" aria-hidden="true"></i>
        </h5>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Testimonials",
};
</script>

<style lang="scss">
@import "@/assets/styles/variables.scss";

.testimonials {
  background-image: linear-gradient($my-lightblue, white);
  img {
    width: 100%;
  }
  .w-50 {
    margin-top: -5rem;
  }
  p {
    color: $my-gray;
  }
  .col-5 {
    background-image: url("../assets/img/mark.png");
    background-size: 30%;
    background-repeat: no-repeat;
    background-position: center;
    background-color: white;
    background-blend-mode: luminosity;
    box-shadow: 0 10px 20px $my-gray;
    position: relative;
    cursor: pointer;
    transition: transform 0.3s;
    &:hover {
      transform: scale(1.1);
    }
    &::after {
      position: absolute;
      bottom: -1rem;
      content: "";
      box-shadow: 0 10px 20px $my-gray;
      height: 1rem;
      width: 90%;
    }
    img {
      width: 20%;
      margin-top: 2.5rem;
    }
    span {
      font-size: 1.1rem;
      color: $my-gray;
    }
  }
  h5 {
    display: inline-block;
    padding: 0.4rem;
    cursor: pointer;
    &:focus {
      color: $my-blue;
    }
  }
}
</style>
