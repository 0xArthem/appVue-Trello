<template>
  <router-link class="board-card" :to="{ name: 'board', params: { name, id } }">
    <span class="board-card-title">
      {{ name }}
    </span>
  </router-link>
</template>

<script>
export default {
  name: "board-card",
  props: {
    id: String,
    name: String,
  },
};
</script>

<style lang="scss" scoped></style>
