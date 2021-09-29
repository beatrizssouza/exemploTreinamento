<template>
  <div id="app">
    <NovoComponente />
  </div>
</template>

<script>
import NovoComponente from "./components/NovoComponente.vue";

export default {
  name: "App",
  components: {
    NovoComponente,
  },
};
</script>

<style>
#app {
  margin: 0;
  background-color: white;
}
</style>
