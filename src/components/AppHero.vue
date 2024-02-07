<script>
export default {
  data() {
    return {
      imgName: "vite-vue.webp",
    };
  },
  methods: {
    /**
     * Funzione che restituisce il path assoluto che VUE non riesce a comprendere da solo
     * @param {*} imgName path relativo
     */
    getUrl(imgName) {
      const imgUrl = new URL("../assets/img/" + imgName, import.meta.url);
      return imgUrl.href;
    },
  },
};
</script>

<template>
  <div class="wrapper">
    <img :src="getUrl(imgName)" alt="" class="hero" />
  </div>
</template>

<!-- Scoped fa si che le classi inserite qui sottovalgano solo e soltanto per questo componente-->
<style scoped>
.wrapper {
  width: 100%;
}
.hero {
  width: 100%;
  border: 3px solid black;
}
</style>
