<template>
  <div class="container-fluid">
    <div class="container">
      <h1>→ Content goes here ←</h1>
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
  background: #1c1c1c;

  .container {
    width: 1000px;
    min-height: 100px;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
    color: #fffffd;
  }
}
</style>