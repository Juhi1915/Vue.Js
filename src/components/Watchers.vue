<template>
  <div>
    <hr />
    <hr />
    <h2>Volume Tracker(0-20)</h2>
    <h4>Current Value - {{ volume }}</h4>
    <div>
      <button @click="volume += 2">Increase</button>
      <button @click="volume -= 1">Decrease</button>
    </div>
    <div>
      <input type="text" v-model="movie" />
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      volume: 0,
      movie: "",
    };
  },
  methods: {},
  computed: {},
  watch: {
    volume(newValue, oldvalue) {
      if (newValue > oldvalue && newValue === 16) {
        alert("Listing high volume for long time may damage your hearing");
      }
    },
    //if we have single object Using mmediate we can get api during Page load
    //But if we have nested object in that case we need to use deep watchers
    movie: {
      handler(newvalue) {
        console.log(`API Call when page load:- ${newvalue}`);
      },
      immediate: true,
    },
  },
};
</script>