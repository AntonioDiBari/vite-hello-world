<script>
/* Esporto i componenti dal file */
import AppTitle from "./components/AppTitle.vue";
import AppHero from "./components/AppHero.vue";

export default {
  data() {
    return {};
  },
  /* Aggiungo i componenti con questa chiave di Vue */
  components: { AppTitle: AppTitle, AppHero },
};
</script>

<template>
  <!-- Utilizzo i componenti con un tag con il nome dato nei data -->
  <AppTitle />
  <AppHero />
</template>

<style>
/* Nell'app main linko il css */
@import URL("./assets/main.css");
</style>
