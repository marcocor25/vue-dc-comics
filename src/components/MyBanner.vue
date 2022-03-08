<template>
  <div class="container-fluid">
    <div class="container">
      <div class="thumb-wrapper">
        <figure class="thumb-image">
          <img src="../assets/img/buy-comics-digital-comics.png" />
        </figure>
        <h4>digital comics</h4>
      </div>
      <div class="thumb-wrapper">
        <figure class="thumb-image">
          <img src="../assets/img/buy-comics-merchandise.png" />
        </figure>
        <h4>dc merchandise</h4>
      </div>
      <div class="thumb-wrapper">
        <figure class="thumb-image">
          <img src="../assets/img/buy-comics-subscriptions.png" />
        </figure>
        <h4>subscription</h4>
      </div>
      <div class="thumb-wrapper">
        <figure class="thumb-image">
          <img src="../assets/img/buy-comics-shop-locator.png" />
        </figure>
        <h4>comic shop locator</h4>
      </div>
      <div class="thumb-wrapper">
        <figure class="thumb-image">
          <img src="../assets/img/buy-dc-power-visa.svg" />
        </figure>
        <h4>dc power visa</h4>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "MyMain",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.container-fluid {
  background: #0082f9;

  .container {
    width: 950px;
    min-height: 130px;
    display: flex;
    justify-content: space-between;
    margin: 0 auto;
    color: #fffffd;

    .thumb-wrapper {
      display: flex;
      align-items: center;
      gap: 10px;
      cursor: pointer;

      .thumb-image {
        width: 50px;
        height: 50px;

        img {
          object-fit: contain;
        }
      }

      h4 {
        text-transform: uppercase;
      }
    }
  }
}
</style>