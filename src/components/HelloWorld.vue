<template>
  <div>
    <h1>Hello Computed Properties:- {{fullName}}</h1>
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
      firstName:'Juhi',
      lastName:'Bhardwaj'
    };
  },
  computed: {
    fullName(){
      return `${this.firstName}  ${this.lastName}`
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->

