<template>
  <div id="app">
    <Header />
    <H1>The Advocate </H1>
    <!-- <Newsfeed /> -->
  </div>
</template>

<script>
import Header from "./components/Header";
// import Newsfeed from "./components/Newsfeed";

export default {
  name: "App",
  components: {
    Header,
    // Newsfeed,
  },
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
