<template>
  <Expressions></Expressions>
  <hr />
  <Directives></Directives>
  <hr />
  <Binding></Binding>
  <hr />
  <list-rendering></list-rendering>
  <hr />
  <actions-events></actions-events>
</template>

<script>
import Expressions from "./components/Expressions.vue";
import Directives from "./components/Directives.vue";
import Binding from "./components/Binding.vue";
import ListRendering from "./components/ListRendering.vue";
import ActionsEvents from "./components/ActionsEvents.vue";

export default {
  name: "App",
  components: {
    Expressions,
    Directives,
    Binding,
    ListRendering,
    ActionsEvents,
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
  margin-top: 60px;
}
</style>
