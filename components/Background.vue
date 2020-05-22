<template>
  <div class="background-wrapper">
    <div class="circle-1"></div>
    <div class="circle-2"></div>
    <div class="circle-3"></div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped lang="scss">
.background-wrapper {
  background-color: $base-color;
  z-index: -1;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  /* max-height: 100%; */
  min-height: 100vh;
  position: absolute;
  overflow: hidden;
}
.circle-1 {
  position: absolute;
  width: 242px;
  height: 242px;
  left: 647px;
  top: 150px;
  border-radius: 50%;
  background: rgba(60, 90, 159, 0.1);
}
.circle-2 {
  position: absolute;
  width: 343px;
  height: 343px;
  left: 47px;
  top: 555px;
  border-radius: 50%;
  background: rgba(188, 58, 128, 0.1);
}
.circle-3 {
  position: absolute;
  width: 543px;
  height: 543px;
  left: 1001px;
  top: 500px;
  border-radius: 50%;
  background: rgba(60, 90, 159, 0.1);
}
</style>
