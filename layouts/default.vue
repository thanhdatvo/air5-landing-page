<template>
  <div class="app-wrapper">
    <navigation-bar />
    <nuxt />
    <background />
  </div>
</template>

<script>
export default {
  components: {
    'navigation-bar': () => import('~/components/NavigationBar.vue'),
    background: () => import('~/components/Background.vue')
  }
}
</script>
<style lang="scss">
html {
  font-family: 'Poppins', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-size: 40%;
  word-spacing: 1px;
  // -ms-text-size-adjust: 100%;
  // -webkit-text-size-adjust: 100%;
  // -moz-osx-font-smoothing: grayscale;
  // -webkit-font-smoothing: antialiased;
  box-sizing: border-box;

  @include media-breakpoint-up(md) {
    font-size: 62.5%;
  }
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
  color: white;
}
.app-wrapper {
  position: relative;
}
</style>
