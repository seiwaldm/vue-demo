<template>
  <Expressions></Expressions>
  <hr />
  <Directives></Directives>
  <hr />
  <Binding></Binding>
  <hr />
  <list-rendering></list-rendering>
</template>

<script>
import Expressions from "./components/Expressions.vue";
import Directives from "./components/Directives.vue";
import Binding from "./components/Binding.vue";
import ListRendering from "./components/ListRendering.vue";

export default {
  name: "App",
  components: { Expressions, Directives, Binding, ListRendering },
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
