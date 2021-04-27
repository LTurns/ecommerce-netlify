<template>
  <section>
    <ul>
      <li>About</li>
      <li>Company</li>
      <li>Locations</li>
      <li>Contact</li>
      <li>Hours</li>
    </ul>
    <ul>
      <li>Twitter</li>
      <li>Facebook</li>
      <li>Instagram</li>
      <li>LinkedIn</li>
    </ul>
    <ul>
      <h4>Catalogue</h4>
      <a href="http://www.cbsproducts.com/wp-content/uploads/2021/03/CBS-Main-Product-Catalogue.pdf">Download Catalogue</a>
    </ul>
  </section>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
section {
  width: 80%;
  margin-left: 10%;
  padding: 40px 0;
  display: grid;
  grid-template-columns: repeat(3, 1fr);
}

ul {
  list-style: none;
  padding-left: 0;
}

input {
  width: 100%;
}

@media screen and (min-width: 850px) {
  section {
    padding: 40px !important;
  }
}
</style>