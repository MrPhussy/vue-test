<template>
  <div id="app">
    <img alt="Vue logo" src="https://vuejs.org/images/logo.png" />
    <nav>
      <a href="#dashboard">Dashboard</a> |
      <a href="#lessonPlanner">Lesson Planner</a> |
      <a href="#history">History</a>
    </nav>
    <HelloWorld msg="Welcome to Your Vue.js App" />
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue';

export default {
  name: 'App',
  components: {
    HelloWorld,
  },
  data() {
    return {
      navLinks: ['#dashboard', '#lessonPlanner', '#history'],
    };
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoying: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 10px;
}

nav a {
  color: #2c3e50;
  text-decoration: none;
}

nav a:hover {
  background-color: rgba(49, 74, 116, 0.2);
}
</style>
