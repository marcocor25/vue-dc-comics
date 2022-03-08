<template>
  <div class="container-fluid">
    <div class="container">
      <div class="button">sign-up now</div>

      <div class="social-wrapper">
        <h3>follow us</h3>
        <div class="icons-wrapper">
          <figure class="icon">
            <img src="../assets/img/footer-facebook.png" />
          </figure>
          <figure class="icon">
            <img src="../assets/img/footer-twitter.png" />
          </figure>
          <figure class="icon">
            <img src="../assets/img/footer-youtube.png" />
          </figure>
          <figure class="icon">
            <img src="../assets/img/footer-pinterest.png" />
          </figure>
          <figure class="icon">
            <img src="../assets/img/footer-periscope.png" />
          </figure>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "FooterBanner",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.container-fluid {
  background: #303030;

  .container {
    width: 1000px;
    min-height: 80px;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;

    .button {
      padding: 10px;
      border: 2px solid #0c80f7;
      text-transform: uppercase;
      cursor: pointer;
      color: #fffffd;
    }

    .social-wrapper {
      display: flex;
      align-items: center;
      gap: 20px;
      text-transform: uppercase;
      color: #0c80f7;
    }

    .icons-wrapper {
      display: flex;
      gap: 10px;
    }

    .icon {
      width: 25px;
      height: 25px;
      cursor: pointer;
    }
  }
}
</style>