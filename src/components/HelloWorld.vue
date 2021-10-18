<template>
  <div>
    Hello {{ name }}
    <div v-html="channel"></div>
    <!-- {Surthod property} -->
    <button :disabled="isDisabled">Code Sendbox</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      name: "Juhi Bhardwaj",
      channel: "<b>Code Sendbox</b>",
      isDisabled: true,
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->

