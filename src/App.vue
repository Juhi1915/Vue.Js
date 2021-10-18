<template>
  <div id="app">
    <HelloWorld msg="Hello Vue in CodeSandbox!" />
    <ConditionalRendering />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld";
import ConditionalRendering from "./components/ConditionalRendering";

export default {
  name: "App",
  components: {
    HelloWorld,
    ConditionalRendering,
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
