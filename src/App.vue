<template>
  <div id="app">
    <Carousel></Carousel>
    <Navbar></Navbar>
    <router-view/>
    <SocialMedia></SocialMedia>
  </div>
</template>
<script>
import Carousel from '@/components/Carousel.vue'
import Navbar from '@/components/Navbar.vue'
import SocialMedia from '@/components/SocialMedia.vue'
export default {
  name: 'App',
  components: {
    Carousel,
    Navbar,
    SocialMedia
  }
}
</script>

<style>
</style>
