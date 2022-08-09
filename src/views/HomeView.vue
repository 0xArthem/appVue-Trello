<template>
  <div class="home">
    <app-home />
  </div>
</template>

<script>
import AppHome from "@/components/AppHome";
export default {
  name: "HomeView",
  components: {
    AppHome,
  },
};
</script>

<style lang="scss" scoped>
* {
  background-color: #2e91d5;
}
</style>
