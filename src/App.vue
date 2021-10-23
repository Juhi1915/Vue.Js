<template>
  <div id="app">
    <HelloWorld msg="Hello Vue in CodeSandbox!" />
    <ConditionalRendering />
    <NameChnageHandler />
    <Count />
    <Form />
    <Watchers />
    <Greet name="ReactJs" heroname="Batman" />
    <!-- <Greet name="vuejs" heroname="Postman" />
    <Greet name="NodeJs" heroname="NavMan" /> -->
    <Greet :name="name" :heroname="channel" />
    <hr />
    <hr />
    <button @click="showPopup = true">Show Popup</button>
    <CustomExample v-show="showPopup" @close="showPopup = false" />
    <hr />
    <hr />
    <Card>Card Content -1</Card>
    <Card><h2>Card Content -1</h2></Card>
    <Card><img src="./assets/logo.png" /></Card>
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
import CustomExample from "./components/CustomExample";
import Card from "./components/Card";

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
    CustomExample,
    Card,
  },
  data() {
    return {
      name: "Java",
      channel: "GFG",
      showPopup: false,
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
