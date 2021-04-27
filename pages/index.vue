<template>
  <div name="img">
    <app-textlockup />
    <app-sales-boxes />
    <!-- <app-textlockup> -->
      <!-- <template v-slot:img>
        <img src="/bag.jpg" alt="bag" />
      </template> -->
      <!-- <template v-slot:sale>Featured Products</template> -->
    <!-- </app-textlockup> -->
    <app-featured-products />
  </div>
</template>

<script>
import AppTextlockup from "~/components/AppTextlockup.vue";
import AppSalesBoxes from "~/components/AppSalesBoxes.vue";
import AppFeaturedProducts from "~/components/AppFeaturedProducts.vue";

export default {
  components: {
    AppTextlockup,
    AppSalesBoxes,
    AppFeaturedProducts
  }
};
</script>

<style>
.test {
  margin: 3vh;
}

img {
  background-image: '../static/background.jpg'
}

main {
  width: 75vw;
}
</style>
