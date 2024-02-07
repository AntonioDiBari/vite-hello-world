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
  <div>
    <img :src="getUrl(imgName)" alt="" />
  </div>
</template>

<style scoped></style>
