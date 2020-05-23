<template>
  <div class="column">
    <page-1 />
    <page-2 />
    <page-3 />
  </div>
</template>

<script>
export default {
  components: {
    'page-1': () => import('~/components/Page1.vue'),
    'page-2': () => import('~/components/Page2.vue'),
    'page-3': () => import('~/components/Page3.vue')
  }
}
</script>

<style scoped lang="scss"></style>
