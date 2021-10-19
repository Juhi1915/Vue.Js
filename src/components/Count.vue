<template>
  <div>
    <p>***Count :-- Increament Decreament***</p>
    <h3>{{ count }}</h3>
    <button v-on:click="count = count + 1">Increament</button>
    <button v-on:click="count = count - 1">Decreament</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      count: 0,
    };
  },
};
</script>