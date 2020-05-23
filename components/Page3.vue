<template>
  <div id="page3" class="page-wrapper row">
    <div class="title-wrapper col-12 col-lg-6">
      <h1>
        Join
        <span>AIR5.</span>
      </h1>
    </div>
    <div class="form-wrapper col-12 col-lg-6">
      <form action class="column">
        <label for="name">Name</label>
        <input type="text" />
        <label for="email">Email</label>
        <input type="email" />
        <label for="password">Password</label>
        <input type="password" />
        <a-button class="button">Join now</a-button>
      </form>
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
.row {
  margin: 0;
}

.title-wrapper {
  margin-top: 12rem;
  margin-bottom: 20rem;
  h1 {
    min-width: 40rem;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    font-weight: 600;
    font-size: 7.2rem;
    text-align: center;
    span {
      font-size: 9.6rem;
      color: $primary-color;
    }
  }
}
.form-wrapper {
  form {
    background-color: $dark-color;
    padding: 2rem 3rem;
    @include media-breakpoint-up(md) {
      padding: 4rem 6rem;
    }
    label {
      margin-top: 2.4rem;
      display: block;
      font-size: 2.4rem;
      font-weight: 500;
    }
    input {
      margin-top: 2.2rem;
      font-size: 2.4rem;
      display: block;
      width: 100%;
      max-width: 80rem;
      background-color: $dark-color;
      color: white;
      border: 2px solid $secondary-color;
      border-radius: 7px;
      padding: 1.2rem;
    }
    .button {
      margin-top: 6rem;
      display: block;
      text-align: center;
      margin-bottom: 2.4rem;
    }
  }
}
</style>
