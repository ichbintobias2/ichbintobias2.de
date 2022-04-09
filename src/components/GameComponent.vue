<template>
  <h1>{{ title }}</h1>
  <img v-bind:src="'data:image/jpeg;base64,' + image" />
  <img v-bind:src="rating + '-Stars.png'" />
</template>

<script>
export default {
  name: 'GameComponent',
  components: {},
  props: ['title'],
  data () {
    return {
      image: '',
      rating: ''
    }
  },
  mounted () {
    this.getImageAndRating()
  },
  methods: {
    async getImageAndRating () {
      const response = await fetch('sample_rating.json')
      const data = await response.json()
      this.image = data.image
      this.rating = data.rating
    }
  }
}
</script>

<style scoped>
h1 {
  text-align: center;
}

img {
  display: block;
  margin-left: auto;
  margin-right: auto;
}
</style>
