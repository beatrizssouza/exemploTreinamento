<template>
  <div id="App">
    <TesteEvento />
  </div>
</template>

<script>
import TesteEvento from "./components/TesteEvento.vue";

export default {
  name: "App",
  components: {
    TesteEvento,
  },
};
</script>

<style>
#App {
  margin: 0;
  background-color: white;
}
</style>
