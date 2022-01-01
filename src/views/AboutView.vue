<template>
  <div class="about">
    <About/>
  </div>
</template>

<script>
import About from '@/components/about/about.vue'

export default {
  name: 'AboutView',
  components: {
    About
  }
}
</script>

<style lang="scss" scoped>
.about {
  margin-top: 60px;
}
</style>
