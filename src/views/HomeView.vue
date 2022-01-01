<template>
  <div class="home">
    <Main/>
  </div>
</template>

<script>
// @ is an alias to /src
import Main from '@/components/main/main.vue'

export default {
  name: 'HomeView',
  components: {
    Main
  }
}
</script>

<style lang="scss" scoped>
.home{
  margin-top: 60px;
}
</style>
