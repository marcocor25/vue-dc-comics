<template>
  <div id="app">
    <MyHeader />
    <MyMain />
    <MyFooter />
  </div>
</template>

<script>
import MyHeader from "./components/MyHeader.vue";
import MyMain from "./components/MyMain.vue";
import MyFooter from "./components/MyFooter.vue";

export default {
  name: "App",
  components: {
    MyHeader,
    MyMain,
    MyFooter,
  },
};
</script>

<style lang="scss">
#app {
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }

  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
</style>
