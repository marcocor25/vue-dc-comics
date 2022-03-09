<template>
  <div class="card">
    <figure class="card-image">
      <img :src="img" :alt="title" />
    </figure>
    <h5 class="card-title">
      {{ title }}
    </h5>
  </div>
</template>

<script>
export default {
  name: "MyThumbs",
  props: {
    img: String,
    title: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.card {
  width: calc((100% / 6) - 20px);
  height: 190px;
  filter: drop-shadow(2px 2px 3px black);
  cursor: pointer;
  transition: 200ms linear;

  .card-image {
    aspect-ratio: 1/1;

    img {
      object-fit: cover;
      object-position: top;
      display: block;
    }
  }

  .card-title {
    padding: 10px 0;
    text-transform: uppercase;
  }

  &:hover {
    transform: translateY(-10px);
  }
}
</style>
