<template>
  <div id="app">
    <Navbar />
    <transition-group name="fade">
      <router-view key="routes" />
    </transition-group>
    <Footer />
  </div>
</template>
<script>
import Navbar from "./components/partials/Navbar";
import Footer from "./components/partials/Footer";

export default {
  components: { Navbar, Footer }
};
</script>
<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
