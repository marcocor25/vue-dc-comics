<template>
  <div id="app">
    <MyHeader />
    <MyMain />
    <MyBanner />
    <MyFooter />
    <FooterBanner />
  </div>
</template>

<script>
import MyHeader from "./components/MyHeader.vue";
import MyMain from "./components/MyMain.vue";
import MyBanner from "./components/MyBanner.vue";
import MyFooter from "./components/MyFooter.vue";
import FooterBanner from "./components/FooterBanner.vue";

export default {
  name: "App",
  components: {
    MyHeader,
    MyMain,
    MyBanner,
    MyFooter,
    FooterBanner,
  },
};
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

img {
  width: 100%;
  height: 100%;
}

ul {
  list-style: none;
}

#app {
  display: flex;
  flex-direction: column;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  font-size: 12px;
  color: #2c3e50;
}
</style>
