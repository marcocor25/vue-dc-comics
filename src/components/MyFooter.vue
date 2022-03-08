<template>
  <div class="container-fluid">
    <div class="container">
      <div class="list-col">
        <div class="list-wrapper">
          <ul>
            <h2>dc comics</h2>
            <li>Characters</li>
            <li>Comics</li>
            <li>Movie</li>
            <li>TV</li>
            <li>Games</li>
            <li>Videos</li>
            <li>News</li>
          </ul>

          <ul>
            <h2>shop</h2>
            <li>Shop DC</li>
            <li>Shop DC Collectibles</li>
          </ul>
        </div>
        <ul>
          <h2>dc</h2>
          <li>Terms Of Use</li>
          <li>Privacy Policy (New)</li>
          <li>Ad Choices</li>
          <li>Advertising</li>
          <li>Jobs</li>
          <li>Subscription</li>
          <li>Talent Workshops</li>
          <li>CPSC Certificates</li>
          <li>Ratings</li>
          <li>Shop Help</li>
          <li>Contact Us</li>
        </ul>
        <ul>
          <h2>sites</h2>
          <li>DC</li>
          <li>MAD Magazine</li>
          <li>DC Kids</li>
          <li>DC Universe</li>
          <li>DC Power Visa</li>
        </ul>
      </div>

      <div class="logo-col"></div>
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
  background-image: url("../assets/img/footer-bg.jpg");
  background-size: cover;
  background-position: center;

  .container {
    width: 1000px;
    min-height: 300px;
    margin: 0 auto;
    display: flex;
    color: #fffffd;

    .list-col {
      width: 60%;
      padding: 20px 0;
      display: flex;
      gap: 30px;

      h2 {
        padding: 10px 0;
        text-transform: uppercase;
      }

      li {
        cursor: pointer;
        color: #788d77;
      }
    }

    .logo-col {
      width: 40%;
      background-image: url("../assets/img/dc-logo-bg.png");
      background-size: cover;
      background-position: center;
    }
  }
}
</style>