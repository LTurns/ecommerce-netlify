<template>
  <div>
    <app-sales-boxes :data="boxes" />
    <app-sales-boxes :data="boxes" />
  </div>
</template>

<script>
import { mapState } from "vuex";
import AppSalesBoxes from "~/components/AppSalesBoxes.vue";

export default {
  components: {
    AppSalesBoxes
  },
  computed: {
    ...mapState(["storedata"])
  },
  data() {
    return {
      newBoxes: [
        {
          icon: "/icon-package.svg",
          heading: "Product 3",
          details: "Description 3"
        },
        {
          icon: "/icon-cal.svg",
          heading: "Product 1",
          details: "Description 1"
        },
        {
          icon: "/icon-service.svg",
          heading: "Product 2",
          details: "Description 2"
        }
      ]
    };
  }
};
</script>

<style lang="scss" scoped>
</style>