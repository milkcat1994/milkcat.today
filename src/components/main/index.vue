<template>
  <div id="main">
      <ProjectCard/>
      <ProjectCard/>
      <ProjectCard/>
      <ProjectCard/>
  </div>
</template>

<script>
import ProjectCard from '@/components/projectCard/index.vue'

export default {
  components: {
    ProjectCard
  }
}
</script>

<style lang="scss" scoped>
@import './index.scss';

</style>>
