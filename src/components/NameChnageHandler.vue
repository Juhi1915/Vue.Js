<template>
  <div>
    <p>***By click on Button Handler will Change***</p>
    <h3>{{ name }}</h3>
    <button v-on:click="name = 'Vue.Js'">Change name</button>
    <button v-on:mouseover="name = 'Database'">Change Database</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      name: "React Js",
    };
  },
};
</script>