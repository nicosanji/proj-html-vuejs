<template>
  <div class="contact container my-5" id="contact-us">
    <div class="w-50 mx-auto">
      <h2 class="text-center">Contact with our Team</h2>
      <p class="text-center mt-4 mb-5">
        If you are planning on developing a product landing.
      </p>
    </div>
    <div class="row pt-5">
      <div class="col-6 position-relative h-100">
        <div
          class="map-box col-7 d-flex position-absolute bg-white rounded-1 p-2"
        >
          <div class="col-9 d-flex flex-column">
            <div class="map-box-title">Storey Ave</div>
            <div class="map-box-subtitle pb-4">
              San Francisco, California 94126
            </div>
            <a href="maps">Visualizza mappa più grande</a>
          </div>
          <div class="col-3 d-flex flex-column align-items-center">
            <h2 class="mb-0">
              <i class="fa fa-random" aria-hidden="true"></i>
            </h2>
            <a class="px-2" href="indicazioni">Indicazi...</a>
          </div>
        </div>
        <img
          class="w-100"
          src="../assets/img/StaticMapService.GetMapIma.png"
          alt="map-img"
        />
        <div
          class="
            map-zoom
            d-flex
            flex-column
            align-items-center
            position-absolute
            bg-white
            rounded-1
            py-1
            px-2
          "
        >
          <h4 class="mb-0 border-bottom">
            <i class="fa fa-plus" aria-hidden="true"></i>
          </h4>
          <h4 class="mb-0 border-top">
            <i class="fa fa-minus" aria-hidden="true"></i>
          </h4>
        </div>
        <div class="map-location position-absolute">
          <h1 class="mb-0">
            <i class="fa fa-map-marker" aria-hidden="true"></i>
          </h1>
        </div>
      </div>
      <div class="col-6">
        <img src="../assets/img/35.png" alt="logo-png" />
        <h5 class="mt-5 mb-3">9840 Shore St. Fond Du Lac, WI 54936</h5>
        <p class="mb-0">0 1223 456 789</p>
        <p class="mb-5">mail@sofbox.com</p>
        <div class="d-flex mb-5">
          <div class="social-box border rounded-1 text-center me-2">
            <i class="fa fa-facebook" aria-hidden="true"></i>
          </div>
          <div class="social-box border rounded-1 text-center me-2">
            <i class="fa fa-twitter" aria-hidden="true"></i>
          </div>
          <div class="social-box border rounded-1 text-center me-2">
            <i class="fa fa-github" aria-hidden="true"></i>
          </div>
          <div class="social-box border rounded-1 text-center me-2">
            <i class="fa fa-instagram" aria-hidden="true"></i>
          </div>
        </div>
        <h4 class="mb-4">Get in touch</h4>
        <div class="d-flex justify-content-between gap-3 mb-4">
          <input
            class="border rounded p-1 w-50 py-2"
            type="name"
            placeholder=" Your Name"
          />
          <input
            class="border rounded p-1 w-50 py-2"
            type="email"
            placeholder=" Your Email"
          />
        </div>
        <input
          class="border rounded p-1 w-100 mb-4 py-2"
          type="text"
          placeholder=" Your Subject"
        />
        <textarea
          class="border rounded p-1 w-100 mb-4 py-2"
          placeholder=" Your Message"
          cols="30"
          rows="10"
        ></textarea>
        <button type="button" class="btn text-white px-3 py-2 mb-5">
          Send Message
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Contact",
};
</script>

<style lang="scss">
@import "@/assets/styles/variables.scss";

.contact {
  p {
    color: $my-gray;
  }
  .map-box {
    top: 1rem;
    left: 2rem;
    .map-box-title {
      font-size: 1rem;
      font-weight: 600;
    }
    .map-box-subtitle {
      font-size: 0.9rem;
      color: #495057;
    }
    a {
      font-size: 0.9rem;
      color: $my-blue;
    }
    h2 {
      color: $my-blue;
      transform: rotate(270deg);
    }
  }
  .map-zoom {
    bottom: 1rem;
    right: 1.5rem;
    cursor: pointer;
    color: #495057;
  }
  .map-location {
    bottom: 50%;
    right: 50%;
    h1 {
      color: #ff796d;
      font-size: 3.5rem;
    }
  }
  .social-box {
    color: $my-blue;
    width: 2.5rem;
    height: 2.5rem;
    line-height: 2.5rem;
    font-size: 1.25rem;
    cursor: pointer;
    transition: 0.3s;
    &:hover {
      color: white;
      background-color: $my-blue;
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
