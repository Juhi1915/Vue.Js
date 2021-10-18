<template>
  <div>
    <div v-if="num === 0">Conditional Rendering :- Num 0</div>
    <h4 v-else-if="num < 0">Num is Negative</h4>
    <h4 v-else-if="num > 0">Num is Postive</h4>
    <h2 v-else>Not a number</h2>
    <!-- when we have multiple statemnet then we can wrap like this we
    wrap  into template -->
    <template v-if="display">
      <h5>Juhi</h5>
      <h5>Bhardwaj</h5>
      <h5>Vue.js</h5>
    </template>
    <h2 v-show="showItem">V-show</h2>
    <template>
      <h1 v-for="(name, index) in names" :key="index">{{ name }}</h1>
      <h3 v-for="name in fullNames" :key="name">
        {{ name.fisrt }} {{ name.last }}
      </h3>
    </template>
  </div>
</template>


<script>
export default {
  data() {
    return {
      num: 1,
      display: true,
      showItem: true,
      names: ["List Rendering"],
      fullNames: [
        { fisrt: "Juhi", last: "Bhardwaj" },
        { fisrt: "Rohit", last: "Thakur" },
        { fisrt: "Mohit", last: "Bhardwaj" },
      ],
    };
  },
};
</script>