<template>
  <div>
    <hr />
    <hr />
    <h5>{{ name }} a.ke.a -> {{ heroname }}</h5>
  </div>
</template>


<script>
export default {
  name: "component Props",
  props: ["name", "heroname"],
  //BY this way we can add props type in props
  // props: {
  //   title: String
  //   }
  // Or we can also pass required if the props is necessary
  // props: {
  //   title: {
  //   type: "String",
  //   required: true
  // }
  //   }
};
</script>

<style scoped>
</style>