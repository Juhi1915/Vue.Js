<template>
  <div id="app">
    <HelloWorld msg="Hello Vue in CodeSandbox!" />
    <ConditionalRendering />
    <NameChnageHandler />
    <Count />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld";
import ConditionalRendering from "./components/ConditionalRendering";
import NameChnageHandler from "./components/NameChnageHandler";
import Count from "./components/Count";

export default {
  name: "App",
  components: {
    HelloWorld,
    ConditionalRendering,
    NameChnageHandler,
    Count,
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
