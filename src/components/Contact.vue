<template>
  <div class="contact container my-5">
    <div class="row">
      <div class="col-6 position-relative">
        <div
          class="map-box col-7 d-flex position-absolute bg-white rounded-1 p-2"
        >
          <div class="col-9 d-flex flex-column">
            <div class="map-box-title">Storey Ave</div>
            <div class="map-box-subtitle pb-4">
              San Francisco, California 94126
            </div>
            <a href="#">Visualizza mappa più grande</a>
          </div>
          <div class="col-3 d-flex flex-column align-items-center">
            <h1 class="mb-0">
              <i class="fa fa-random" aria-hidden="true"></i>
            </h1>
            <a class="px-2" href="#">Indicazi...</a>
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
        <!-- continua -->
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Contact",
};
</script>

<style></style>
