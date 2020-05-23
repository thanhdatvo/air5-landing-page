<template>
  <div id="page2" class="page-wrapper row">
    <div class="title-wrapper col-12 col-lg-8">
      <h1>
        Experience
        <br />AR furnitures
      </h1>
      <div class="feature-wrapper row">
        <div class="feature col-12 col-md-4">
          <div class="column">
            <img src="/icons/ar.png" alt />
            <span>AR</span>
          </div>
        </div>
        <div class="feature col-12 col-md-4">
          <div class="column">
            <img src="/icons/recommendation.png" alt />
            <span>Recommendation</span>
          </div>
        </div>
        <div class="feature col-12 col-md-4">
          <div class="column">
            <img src="/icons/more.png" alt />
            <span>More</span>
          </div>
        </div>
      </div>
      <h2>
        By joining you can benefit by experience your wishing furniture without
        coming to store
      </h2>
    </div>
    <div class="img-wrapper column col-12 col-lg-4">
      <img src="/pictures/picture1.jpg" alt />
      <img src="/pictures/picture2.jpg" alt />
      <div style=" clear: both;"></div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped lang="scss">
.row {
  margin: 0;
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
  padding-bottom: 15rem;
  text-align: center;
  display: block;
  margin: auto;
  @include media-breakpoint-up(md) {
    margin: 0px;
    text-align: left;
  }
}
.img-wrapper {
  img {
    width: 100%;
    height: auto;
    border-radius: 0.9rem;
    margin-top: 3.5rem;
  }
}
.feature-wrapper {
  @include media-breakpoint-up(md) {
    max-width: 80rem;
  }
  padding: 4rem 0rem;
  .feature {
    padding: 2rem 0rem;
    .column {
      padding: 3rem 0rem;
      background-color: $dark-color;
      margin-right: 2.2rem;
      height: 100%;
    }

    img {
      max-width: 7rem;
      height: auto;
      display: block;
      margin: auto;
    }
    span {
      padding-top: 1.4rem;
      margin: auto;
      display: block;
      text-align: center;
      font-size: 2.4rem;
    }
  }
}
</style>
