<template>
  <div class="container-fluid">
    <div class="container">
      <div
        v-for="(element, index) in thumbs"
        :key="index"
        class="thumb-wrapper"
      >
        <figure class="thumb-image">
          <img
            :src="require(`../assets/img/` + element.img)"
            :alt="element.text"
          />
        </figure>
        <h4>{{ element.text }}</h4>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "MyBanner",
  data() {
    return {
      thumbs: [
        {
          img: "buy-comics-digital-comics.png",
          text: "digital comics",
        },
        {
          img: "buy-comics-merchandise.png",
          text: "dc merchandise",
        },
        {
          img: "buy-comics-subscriptions.png",
          text: "subscription",
        },
        {
          img: "buy-comics-shop-locator.png",
          text: "comic shop locator",
        },
        {
          img: "buy-dc-power-visa.svg",
          text: "dc power visa",
        },
      ],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.container-fluid {
  background: #0082f9;
  padding: 20px 0;

  .container {
    width: 1000px;
    min-height: 110px;
    display: flex;
    justify-content: space-between;
    margin: 0 auto;
    padding: 0 20px;
    color: #fffffd;

    .thumb-wrapper {
      display: flex;
      align-items: center;
      padding: 0 10px;
      gap: 10px;
      border-radius: 10px;
      cursor: pointer;
      transition: 200ms linear;

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

      &:hover {
        background: rgba($color: #333, $alpha: 0.2);
      }
    }
  }
}
</style>