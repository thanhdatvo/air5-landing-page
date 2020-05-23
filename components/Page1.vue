<template>
  <div id="page1" class="page-wrapper">
    <div class="title-wrapper">
      <h1>Furniture AR</h1>
      <h2>
        Experience more than thousands
        <br />of furnitures in one app
      </h2>
      <a-button class="button" href="#page2">Join now</a-button>
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
    // timer: () => import('~/components/Timer.vue')
  }
  // asyncData(app) {
  //   return {
  //     starttime: Date.now().toString(),
  //     endtime: new Date().setDate(Date.now().getDate() + 10).toString()
  //   }
  // },
  // data() {
  //   return {
  //     starttime: Date.now().toString(),
  //     endtime: new Date().setDate(Date.now().getDate() + 10).toString()
  //   }
  // }
}
</script>

<style scoped lang="scss">
.button {
  margin: 3px auto;
}

.title-wrapper {
  text-align: center;
  @include media-breakpoint-up(md) {
    text-align: left;
  }
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
  text-align: center;
  display: block;
  margin: auto;
  @include media-breakpoint-up(md) {
    margin: 0px;
    text-align: left;
  }
}
h2 {
  font-weight: 500;
  font-size: 3.6rem;
  max-width: 60rem;
  text-align: center;
  display: block;
  margin: auto;
  @include media-breakpoint-up(md) {
    margin: 0px;
    text-align: left;
  }
}
</style>
