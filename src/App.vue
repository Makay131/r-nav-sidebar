<template>
  <div id="body">
  <Navbar />
  <div id="home__content">Coooontent</div>
  </div>
</template>

<script>
import Navbar from "./components/Navbar.vue";
import './styles/styles.css'

export default {
  name: "App",
  components: {
    Navbar,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

#body {
        position: relative;
        min-height: 100vh;
        width: 100%;
        overflow: hidden;
}

#home__content {
  position: absolute;
  height: 100%;
  width: calc(100% - 240px);
  left: 260px;
  padding: 6px 14px;
}


</style>
