<template>
  <vue-card-stack :cards="cards">
    <template v-slot:card="{ card }">
      <div
        :style="{ background: card.background }"
        style="with: 100%; height: 100%;"
      >
        <p>On The Road</p>
      </div>
    </template>
  </vue-card-stack>
</template>

<script>
import VueCardStack from 'vue-card-stack'
export default {
  components: {
    VueCardStack,
  },
  data() {
    return {
      cards: [
        { background: '#00659d' },
        { background: '#00abbc' },
        { background: '#e2c58a' },
        { background: '#fc8890' },
        { background: '#b35d7f' },
      ],
    }
  },
}
</script>

<style scoped></style>
