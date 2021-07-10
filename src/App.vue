<template>
  <Bootstrap />
  <Card />
</template>

<script>
import Bootstrap from "./components/Bootstrap.vue";
import Card from "./components/Card.vue";

export default {
  name: "App",

  components: {
    Bootstrap,
    Card,
  },
};
</script>

<style>
body {
  font-family: "Futura";
}
</style>
