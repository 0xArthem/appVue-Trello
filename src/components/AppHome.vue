<template>
  <div class="AppHome">
    <h3>Ma liste de tâches</h3>
    <div>
      <input
        type="text"
        placeholder="Ajouter une carte"
        v-model="boardName"
        @keyup.enter="add()"
      />

      <board-card
        v-for="(board, index) in boards"
        :key="index"
        :name="board.name"
        :id="board.id"
      >
      </board-card>
    </div>
  </div>
</template>

<script>
import BoardCard from "@/components/BoardCard";
export default {
  name: "app-home",
  components: { BoardCard },
  data() {
    return {
      boardName: "",
      boards: [
        { id: 1, name: "Tache 1" },
        { id: 2, name: "Tache 2" },
      ],
    };
  },
  methods: {
    add() {
      this.boards.push({ name: this.boardName });
    },
  },
};
</script>

<style lang="scss" scoped>
.AppHome {
  height: 620px;
}
</style>
