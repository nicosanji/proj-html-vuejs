<template>
  <div class="tips-tricks container my-5">
    <div class="row">
      <div class="col-6">
        <h2 class="pe-5 mb-4">
          Get tips tricks on how to skyrocket your sales.
        </h2>
        <p class="mb-4">
          Faff about only a quid blower I don't wanto no agro bleeding chimney
          pot burke tosser cras nice one boot fanny.!
        </p>
        <div tabindex="0" class="evidence-box d-flex px-2 py-3">
          <img src="../assets/img/510.png" alt="repo-analysis" />
          <div class="p-2">
            <h4 class="mb-3">Reporting Analysis</h4>
            <p>
              It is a long established fact that a reader will be distracted by
              the readable content of a page when looking at its layout.
            </p>
          </div>
        </div>
        <div tabindex="0" class="evidence-box d-flex px-2 py-3">
          <img src="../assets/img/511.png" alt="technical-ceo" />
          <div class="p-2">
            <h4 class="mb-3">Technical SEO Audit</h4>
            <p>
              It is a long established fact that a reader will be distracted by
              the readable content of a page when looking at its layout.
            </p>
          </div>
        </div>
      </div>
      <div class="col-6">
        <img src="../assets/img/509.jpeg" alt="sales-img" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "TipsTricks",
};
</script>

<style lang="scss">
@import "@/assets/styles/variables.scss";

.tips-tricks {
  .d-flex {
    img {
      width: 30%;
      height: 30%;
      padding: 1rem;
    }
  }
  .evidence-box {
    cursor: pointer;
    transition: box-shadow 0.3s;
    &:focus {
      border: 1px solid $my-darkgray;
      margin: -1px;
      box-shadow: 10px 20px 20px $my-darkgray;
      h4 {
        color: $my-blue;
      }
    }
  }
  img {
    width: 100%;
  }
  p {
    color: $my-gray;
  }
}
</style>
