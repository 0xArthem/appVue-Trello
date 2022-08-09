<template>
  <h1>Ma liste de tâches</h1>
  <h2>{{ name }}</h2>
</template>

<script>
export default {
  name: "BoardView",
  props: {
    id: String,
    name: String,
  },
};
</script>

<style></style>
