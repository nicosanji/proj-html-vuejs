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
        <div class="evidence-box d-flex px-2 py-3">
          <img src="../assets/img/510.png" alt="repo-analysis" />
          <div class="p-2">
            <h4 class="mb-3">Reporting Analysis</h4>
            <p>
              It is a long established fact that a reader will be distracted by
              the readable content of a page when looking at its layout.
            </p>
          </div>
        </div>
        <div class="d-flex px-2 py-3">
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
.tips-tricks {
  .d-flex {
    img {
      width: 30%;
      height: 30%;
      padding: 1rem;
    }
  }
  .evidence-box {
    border: 1px solid #00000014;
    box-shadow: 10px 20px 20px #00000014;
    h4 {
      color: #377dff;
    }
  }
  img {
    width: 100%;
  }
  p {
    color: #8e989f;
  }
}
</style>
