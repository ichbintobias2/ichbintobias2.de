<template>
  <div class="home">
    <div id="game">
      <GameComponent title="Vue.js" />
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
  div.home {
    min-width: 100%;
    max-width: 100%;
  }

  div {
    float: left;
    min-width: 50%;
    max-width: 50%;
  }
</style>
