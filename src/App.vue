<template>
  <div id="app">
    <NavBar
      name="Logo Name"
      :navLinks="[
        {
          name: 'Home',
          link: '/home',
        },
        { name: 'About', link: '/about' },
        {
          name: 'Contacts',
          link: '/contact',
        },
        {
          name: 'Projects',
          link: '/projects',
        },
      ]"
    />
    <img alt="Vue logo" src="./assets/logo.png" />
    <HelloWorld msg="Welcome to Your Vue.js App" />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import NavBar from "./components/NavBar.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
    NavBar,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin: 0;
  box-sizing: border-box;
}
</style>
