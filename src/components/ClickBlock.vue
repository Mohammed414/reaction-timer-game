<template>
  <div class="block">CLICK ME NOW!</div>
</template>

<script>
export default {
  name: "Click",
  props: ["delay"],
};
</script>

<style>
.block {
  width: 400px;
  background-color: #0faf87;
  border-radius: 20px;
  color: white;
  padding: 100px 0px;
  margin: 30px auto;
}
</style>
