<template>
  <div class="container">
    <figure class="logo">
      <img src="../assets/img/dc-logo.png" />
    </figure>

    <div class="nav-link">
      <ul>
        <li><a href="#">characters</a></li>
        <li><a href="#">comics</a></li>
        <li><a href="#">movies</a></li>
        <li><a href="#">tv</a></li>
        <li><a href="#">games</a></li>
        <li><a href="#">collectibles</a></li>
        <li><a href="#">videos</a></li>
        <li><a href="#">fans</a></li>
        <li><a href="#">news</a></li>
        <li><a href="#">shop</a></li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "MyHeader",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.container {
  min-width: 1000px;
  min-height: 80px;
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
  align-items: center;
  background: white;

  .logo {
    width: 70px;
    height: 70px;
  }

  .nav-link {
    ul {
      display: flex;
      gap: 15px;
    }

    a {
      font-weight: 700;
      text-decoration: none;
      text-transform: uppercase;
      color: currentColor;
    }
  }
}
</style>