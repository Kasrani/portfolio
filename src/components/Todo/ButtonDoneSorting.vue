<template>
  <v-btn
    class="button-done-sorting"
    @click="$store.commit('toggleSorting')"
    color="pink"
  >
      Terminé
  </v-btn>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.button-done-sorting {
    position: fixed;
    bottom: 20px;
    left: 50%;
    transform: translateX(-50%);
}
</style>