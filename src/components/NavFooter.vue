<template>
  <div class="container-fluid">
    <div class="container">
      <div class="button">{{ buttonText }}</div>

      <div class="social-wrapper">
        <h3>{{ socialText }}</h3>
        <div class="icons-wrapper">
          <figure v-for="(element, index) in social" :key="index" class="icon">
            <img
              :src="require(`../assets/img/` + element.img)"
              :alt="element.text"
            />
          </figure>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "NavFooter",
  data() {
    return {
      buttonText: "sign-up now",
      socialText: "follow us",
      social: [
        {
          text: "Facebook",
          img: "footer-facebook.png",
        },
        {
          text: "Twitter",
          img: "footer-twitter.png",
        },
        {
          text: "YouTube",
          img: "footer-youtube.png",
        },
        {
          text: "Pinterest",
          img: "footer-pinterest.png",
        },
        {
          text: "Periscope",
          img: "footer-periscope.png",
        },
      ],
    };
  },
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
      transition: 200ms linear;

      &:hover {
        transform: scale(1.1);
        background: #1e518d;
      }
    }

    .social-wrapper {
      display: flex;
      align-items: center;
      gap: 20px;
      text-transform: uppercase;
      color: #0c80f7;
      cursor: default;
    }

    .icons-wrapper {
      display: flex;
      gap: 10px;
    }

    .icon {
      width: 25px;
      height: 25px;
      cursor: pointer;
      transition: 200ms linear;

      &:hover {
        transform: scale(1.2);
      }
    }
  }
}
</style>