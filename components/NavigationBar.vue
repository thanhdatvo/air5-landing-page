<template>
  <div class="nav-bar">
    <!-- <div id="nav-placeholder" /> -->
    <div class="nav-wrapper">
      <div class="branch row">
        <img id="logo" src="/logo.png" alt="logo" />
        <h1>Air5</h1>
      </div>

      <label for="toggle">&#9776;</label>
      <input id="toggle" ref="menu" type="checkbox" name />

      <div class="menu-wrapper">
        <a href="#page1" @click="toggle()">Discover</a>
        <a href="#page2" @click="toggle()">Join</a>
        <a href="#page3" @click="toggle()">Business</a>
      </div>
      <div style=" clear: both;"></div>
    </div>
  </div>
</template>
<script>
export default {
  methods: {
    toggle() {
      this.$refs.menu.checked = false
    }
  }
}
</script>
<style scoped lang="scss">
.nav-bar {
  #nav-placeholder {
    height: 5rem;
  }
  .nav-wrapper {
    z-index: 1;
    background-color: $base-color;
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    // border-bottom: 1px solid $divider-color;
    padding: 1rem 7rem;
    .branch {
      float: left;
      #logo {
        width: 6rem;
        height: 6rem;
      }
      h1 {
        margin: auto;
        font-size: 3rem;
        margin-left: 10px;
      }
    }

    .menu-wrapper {
      text-align: center;
      display: none;
      height: 100vh;

      width: 100%;
      @include media-breakpoint-up(md) {
        text-align: right;
        display: block;
        height: 100%;
      }
      a {
        line-height: 7rem;
        clear: both;
        text-decoration: none;
        font-size: 2.4rem;
        margin: 0 1rem;
        display: block;
        @include media-breakpoint-up(md) {
          display: inline;
        }
      }
    }
    label {
      float: right;
      font-size: 3rem;
      display: block;
      cursor: pointer;

      @include media-breakpoint-up(md) {
        display: none;
      }
    }
    #toggle {
      display: none;
      &:checked + .menu-wrapper {
        display: block;
      }
    }
  }
}
</style>
