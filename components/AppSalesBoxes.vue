<template>
  <section class="boxes">
    <button v-for="(box, i) in boxes" :key="box.heading" :class="`box${i}`">
      <nuxt-link class="link" exact to="/product-list">
      <img :src="box.icon" alt="service icon" />
       <h4>{{ box.heading }}</h4>
      <p>{{ box.details }}</p>
        </nuxt-link>
    </button>
  </section>
</template>

<script>
export default {
  data() {
    return {
      boxes: [
        {
          icon: "/icon-package.svg",
          heading: "Service 3",
          details: "Description 3"
        },
        {
          icon: "/icon-cal.svg",
          heading: "Service 1",
          details: "Description 1"
        },
        {
          icon: "/icon-service.svg",
          heading: "Service 2",
          details: "Description 2"
        }
      ]
    };
  }
};
</script>

<style lang="scss" scoped>
.boxes {
  margin: 70px 0;
  div {
    border: 1px solid #ddd;
    min-height: 150px;
    justify-self: center;
    align-self: center;
    text-align: center;
  }
  .box1 {
    grid-area: 1 / 1 / 2 / 2;
  }
  .box2 {
    grid-area: 1 / 2 / 2 / 3;
  }
  .box3 {
    grid-area: 1 / 3 / 2 / 4;
  }
  .link {
    color: black;
  }
}

h4 {
  text-transform: uppercase;
  letter-spacing: 0.15em;
  margin: 0 0 10px 0;
}

@media screen and (min-width: 700px) {
  .boxes {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    grid-template-rows: 1fr;
    grid-column-gap: 20px;
    grid-row-gap: 0px;
    div {
      padding: 40px 50px;
    }
  }
}

@media screen and (max-width: 699px) {
  .boxes {
    width: 83vw;
    margin-left: 5vw;
    div {
      padding: 10px 20px;
      margin-bottom: 10px;
    }
  }
}
</style>