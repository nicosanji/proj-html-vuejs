<template>
  <div class="features container-fluid position-relative">
    <img id="circle-img" src="../assets/img/14.png" alt="circle-img" />
    <div class="container pt-5 pb-3">
      <div class="row">
        <div class="col-9">
          <h2 class="mb-4">Popular features that your business needs</h2>
          <p class="pe-5">
            Faff about only a quid blower I don't want no agro bleeding chimney
            pot burke tosser cras nice one boot fanny.!
          </p>
        </div>
        <div class="col-3">
          <button class="btn text-white px-3 py-2 my-5">
            Explore More Feature
          </button>
        </div>
      </div>
      <div class="row mt-5">
        <div class="box col-3 bg-white rounded-1 px-3 py-4">
          <h4>Customized Invoices</h4>
          <h1 class="i-blue">
            <i class="fa fa-line-chart pt-3" aria-hidden="true"></i>
          </h1>
        </div>
        <div class="box col-3 bg-white rounded-1 px-3 py-4">
          <h4>Stock Management</h4>
          <h1 class="i-orange">
            <i class="fa fa-paper-plane-o pt-3" aria-hidden="true"></i>
          </h1>
        </div>
        <div class="box col-3 bg-white rounded-1 px-3 py-4">
          <h4>Receivable & Payables</h4>
          <h1 class="i-green">
            <i class="fa fa-address-card-o pt-3" aria-hidden="true"></i>
          </h1>
        </div>
        <div class="box col-3 bg-white rounded-1 px-3 py-4">
          <h4>Manage Buying</h4>
          <h1 class="i-blue">
            <i class="fa fa-address-book pt-3" aria-hidden="true"></i>
          </h1>
        </div>
        <div class="box col-3 bg-white rounded-1 px-3 py-4">
          <h4>Powerfull & Secure</h4>
          <h1 class="i-orange">
            <i class="fa fa-ravelry pt-3" aria-hidden="true"></i>
          </h1>
        </div>
        <div class="box col-3 bg-white rounded-1 px-3 py-4">
          <h4>Fastest Return Filing</h4>
          <h1 class="i-green">
            <i class="fa fa-address-card-o pt-3" aria-hidden="true"></i>
          </h1>
        </div>
        <div class="box col-3 bg-white rounded-1 px-3 py-4">
          <h4>Monthly Detailed</h4>
          <h1 class="i-blue">
            <i class="fa fa-book pt-3" aria-hidden="true"></i>
          </h1>
        </div>
        <div class="box col-3 bg-white rounded-1 px-3 py-4">
          <h4>Product Management</h4>
          <h1 class="i-orange">
            <i class="fa fa-thumbs-o-up pt-3" aria-hidden="true"></i>
          </h1>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Features",
};
</script>

<style lang="scss">
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
    transition: 0.3s;
    &:hover {
      color: white !important;
      background-color: #6cdac1 !important;
      box-shadow: none;
      h1 {
        color: white;
      }
    }
    h1 {
      font-size: 4rem;
    }
  }
  .i-blue {
    color: #377dff;
  }
  .i-orange {
    color: #ff796d;
  }
  .i-green {
    color: #6cdac1;
  }
}
</style>
