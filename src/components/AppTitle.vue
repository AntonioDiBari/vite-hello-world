<script>
export default {
  data() {
    return {
      title: "La mia prima app con Vite!",
    };
  },
};
</script>

<template>
  <h1 class="title">{{ title }}</h1>
</template>

<!-- Scoped fa si che le classi inserite qui sottovalgano solo e soltanto per questo componente-->

<style scoped></style>
