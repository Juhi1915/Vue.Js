<template>
  <div>
    <hr />
    <hr />
    <h1>{{ name }} a.ke.a -> {{ heroname }}</h1>
  </div>
</template>


<script>
export default {
  name: "component Props",
  props: ["name", "heroname"],
};
</script>

<style scoped>
</style>