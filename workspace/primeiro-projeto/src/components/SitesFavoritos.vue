<template>
  <div class="sites-favoritos">
    <h1>Sites favoritos</h1>

    <ul>
      <li v-for="site of sitesFavoritos" :key="site.id">
        <a :href="site.link"> {{ site.nome }} </a>
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  name: "SitesFavoritos",
  data() {
    return {
      sitesFavoritos: [],
    };
  },
  created() {
    fetch("https://hackthon-decola.firebaseio.com/sites-favoritos.json")
      .then((resultado) => resultado.json())
      .then((json) => {
        this.sitesFavoritos = json;
      });
  },
};
</script>

<style scoped>
</style>