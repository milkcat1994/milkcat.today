<template>
  <div id="about">
    <Dividor title="Milkcat" />
    <AboutCard/>
  </div>
</template>

<script>
import Dividor from '@/components/main/dividor/dividor.vue'
import AboutCard from '@/components/about/aboutCard/aboutCard.vue'

export default {

  components: {
    Dividor,
    AboutCard
  }
}
</script>

<style lang="scss" scoped>
@import './about.scss';

</style>
