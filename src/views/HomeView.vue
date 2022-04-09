<template>
  <div class="home">
    <div id="game">
      <GameComponent />
    </div>
    <div id="review">
      <ReviewComponent />
    </div>
  </div>
</template>

<script>
import GameComponent from '@/components/GameComponent.vue'
import ReviewComponent from '@/components/ReviewComponent.vue'

export default {
  name: 'HomeView',
  components: {
    GameComponent, ReviewComponent
  }
}
</script>

<style scoped>
  div {
    float: left;
    border-width: 50px;
  }
</style>
