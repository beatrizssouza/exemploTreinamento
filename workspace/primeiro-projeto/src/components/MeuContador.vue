<template>
  <div class="meu-contador">
    <h1>Meu contador</h1>
    <h2>A quantidade é: {{ contador }}</h2>
    <button @click="maior">+</button>
    <button @click="menor">-</button>
  </div>
</template>

<script>
export default {
  name: "MeuContador",
  data() {
    return { contador: 0 };
  },
  methods: {
    maior() {
      this.contador++;
    },
    menor() {
      this.contador--;
    },
  },
};
</script>

<style scoped>
</style>