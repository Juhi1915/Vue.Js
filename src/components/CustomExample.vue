<template>
  <div>
    <h1>This is a Popup</h1>
    <button @click="$emit('close')">Close Popup</button>
  </div>
</template>

<script>
export default {
  name: "Popup",
  exist: ["close"],
};
</script>

<style scoped>
</style>