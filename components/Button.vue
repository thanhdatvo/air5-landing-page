<template>
  <a :href="href">
    <slot />
  </a>
</template>
<script>
export default {
  props: ['href']
}
</script>
<style lang="scss" scoped>
a {
  text-decoration: none;
  display: inline-block;
  font-size: 2.4rem;
  background-color: #1762a7;
  border-radius: 0.5rem;
  padding: 1.8rem 5.6rem;
  cursor: pointer;
  &:hover {
    background-color: $secondary-color;
  }
}
</style>
