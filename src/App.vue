<template>
  <Expressions></Expressions>
  <hr />
  <Directives></Directives>
</template>

<script>
import Expressions from "./components/Expressions.vue";
import Directives from "./components/Directives.vue";
export default {
  name: "App",
  components: { Expressions, Directives },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
