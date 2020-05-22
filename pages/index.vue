<template>
  <div class="column" style="height: 1000px">
    <div class="title-wrapper">
      <h1>Furniture AR</h1>
      <h2>
        Experience more than thousands
        <br />of furnitures in one app
      </h2>
      <a-button class="button">Join now</a-button>
    </div>
    <div class="img-wrapper">
      <img src="/pictures/chairs_table.png" alt />
      <div style=" clear: both;"></div>
    </div>
  </div>
</template>

<script>
export default {
  components: {
    'a-button': () => import('~/components/Button.vue')
  }
}
</script>

<style scoped lang="scss">
.button {
  margin-top: 3rem;
}

.title-wrapper {
  padding: 8.5rem 7rem 0rem 7rem;
  width: 800px;
  max-width: 100%;
}

img {
  float: right;
  width: 960px;
  max-width: 100%;

  @include media-breakpoint-up(xl) {
    margin-top: -19rem;
  }
}

h1 {
  font-weight: 600;
  font-size: 7.2rem;
}
h2 {
  font-weight: 500;
  font-size: 3.6rem;
}
</style>
