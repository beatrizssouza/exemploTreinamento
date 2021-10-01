<template>
  <div class="teste-evento">
    <h1>Teste Evento</h1>
    <p @click="deixarMaiuscula">{{ messagem }}</p>
  </div>
</template>

<script>
export default {
  name: "TesteEvento",
  data() {
    return {
      messagem: "o rato roeu a roupa do rei de roma",
    };
  },
  methods: {
    deixarMaiuscula() {
      this.messagem = this.messagem.toUpperCase();
    },
  },
};
</script>

<style scoped>
</style>