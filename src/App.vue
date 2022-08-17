<template>
  <div id="app">
    <ListItem
      :items="[
        'Surface Laptop 2',
        'Google Pixel 4xl',
        'Sony 1000xm4',
        'Desk Lamp',
      ]"
    >
    </ListItem>
    <!-- <Example @click="callingFunction"> Find More Cars </Example> -->
  </div>
</template>
<script>
import ListItem from "./components/ListItem.vue";
// import Example from "./example.js";
export default {
  name: "app",
  components: {
    ListItem,
    // Example,
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Work+Sans&display=swap");
#app {
  font-family: "Work Sans", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: white;
}
</style>
