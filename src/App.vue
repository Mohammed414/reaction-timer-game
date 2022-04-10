<template>
  <h1>Welcome to Reaction Timer Game</h1>
  <button @click="start">START</button>
  <ClickBlock v-if="isPlaying" />
</template>

<script>
import ClickBlock from "./components/ClickBlock.vue";
export default {
  name: "App",
  components: {
    ClickBlock,
  },
  data() {
    return {
      isPlaying: false,
      delay: null,
    };
  },
  methods: {
    start() {
      this.delay = Math.floor(2000 + Math.random() * 4000);
      this.isPlaying = true;
      console.log(this.delay);
    },
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #155391;
  margin-top: 60px;
}
</style>
