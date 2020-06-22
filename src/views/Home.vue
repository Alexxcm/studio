<template>
  <div class="home">
    <Selector/>
  </div>
</template>

<script>
// @ is an alias to /src
import Selector from '@/components/Selector.vue'

export default {
  name: 'Home',
  components: {
    Selector
  }
}
</script>
