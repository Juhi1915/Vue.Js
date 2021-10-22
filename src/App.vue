<template>
  <div id="app">
    <HelloWorld msg="Hello Vue in CodeSandbox!" />
    <ConditionalRendering />
    <NameChnageHandler />
    <Count />
    <Form />
    <Watchers />
    <Greet name="React Js" heroname="Batman" />
    <Greet name="vue js" heroname="Postman" />
    <Greet name="Node Js" heroname="NavMan" />
    <Greet :name="name" :channel="channel" />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld";
import ConditionalRendering from "./components/ConditionalRendering";
import NameChnageHandler from "./components/NameChnageHandler";
import Count from "./components/Count";
import Form from "./components/Form";
import Watchers from "./components/Watchers";
import Greet from "./components/Greet";

export default {
  name: "App",
  components: {
    HelloWorld,
    ConditionalRendering,
    NameChnageHandler,
    Count,
    Form,
    Watchers,
    Greet,
  },
  data() {
    return {
      name: "Java",
      channel: "GFG",
    };
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
