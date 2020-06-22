<template>
  <div>
    <div class="logo"><img thumbnail fluid :src="require('../assets/YeiLetra.png')" alt="Image 3" width="80%" height="20%"></div>
    <b-carousel
      class = "image"
      id="carousel-1"
      v-model="slide"
      :interval="4000"
      controls
      indicators
      background="#ababab"
      style="text-shadow: 1px 1px 2px #333;"
      @sliding-start="onSlideStart"
      @sliding-end="onSlideEnd"
    >
      <!-- Text slides with image -->
      <b-carousel-slide :img-src="require('../assets/ca3.jpg')"
      ></b-carousel-slide>

      <!-- Slides with custom text -->
      <b-carousel-slide :img-src="require('../assets/ca1.jpg')">
      </b-carousel-slide>

      <!-- Slides with image only -->
      <b-carousel-slide :img-src="require('../assets/ca2.jpg')">
      </b-carousel-slide>

    </b-carousel>

  </div>
</template>

<script>
export default {
  name: 'Carousel',
  data () {
    return {
      slide: 0,
      sliding: null
    }
  },
  methods: {
    onSlideStart (slide) {
      this.sliding = true
    },
    onSlideEnd (slide) {
      this.sliding = false
    }
  }
}
</script>
<style scoped>
.logo {
   position: absolute;
   top: 10px;
   z-index: 1;
   text-align: center;
}
</style>
