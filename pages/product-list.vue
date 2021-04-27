<template>
  <div>
    <app-product-boxes-1 />
    <app-product-boxes-2 />
  </div>
</template>

<script>
import { mapState } from "vuex";
import AppProductBoxes1 from "~/components/AppProductBoxes1.vue";
import AppProductBoxes2 from "~/components/AppProductBoxes2.vue";

export default {
  components: {
    AppProductBoxes1,
    AppProductBoxes2
  },
  computed: {
    ...mapState(["storedata"])
  }
};
</script>

<style lang="scss" scoped>
</style>