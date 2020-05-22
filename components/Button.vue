<template>
  <a>
    <slot />
  </a>
</template>
<style lang="scss" scoped>
a {
  display: inline-block;
  font-size: 2.4rem;
  background-color: #1762a7;
  border-radius: 5px;
  padding: 18px 56px;
  cursor: pointer;
  &:hover {
    background-color: #2288e7;
  }
}
</style>
