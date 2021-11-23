<template>
  <div class="online-marketing container my-5 py-5">
    <div class="row mt-5">
      <div class="col-4">
        <div class="d-flex">
          <div><img src="../assets/img/24.png" alt="online-mark" /></div>
          <div class="d-flex flex-column">
            <h4>Online Marketing</h4>
            <p>
              It is a long established fact that a reader will be distracted.
            </p>
            <ul>
              <li v-for="(element, i) in marketingLinks" :key="i">
                <i class="fa fa-check" aria-hidden="true"></i>
                <a href="element.href">{{ element.txt }}</a>
              </li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-4">
        <div class="d-flex">
          <div><img src="../assets/img/24.png" alt="online-mark" /></div>
          <div class="d-flex flex-column">
            <h4>Online Marketing</h4>
            <p>
              It is a long established fact that a reader will be distracted.
            </p>
            <ul>
              <li v-for="(element, i) in marketingLinks" :key="i">
                <i class="fa fa-check" aria-hidden="true"></i>
                <a href="element.href">{{ element.txt }}</a>
              </li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-4">
        <div class="d-flex">
          <div><img src="../assets/img/24.png" alt="online-mark" /></div>
          <div class="d-flex flex-column">
            <h4>Online Marketing</h4>
            <p>
              It is a long established fact that a reader will be distracted.
            </p>
            <ul>
              <li v-for="(element, i) in marketingLinks" :key="i">
                <i class="fa fa-check" aria-hidden="true"></i>
                <a href="element.href">{{ element.txt }}</a>
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

<style></style>
