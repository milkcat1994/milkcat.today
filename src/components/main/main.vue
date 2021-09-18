<template>
  <div id="main">
      <ProjectCard v-for="(project, key) in projects" v-bind:key="key"
      v-bind:pjt="project"
      />
  </div>
</template>

<script>
import ProjectCard from '@/components/projectCard/index.vue'

export default {
  data () {
    return {
      projects: [
        {
          num: 1,
          img: 'https://user-images.githubusercontent.com/18321002/128350386-a12e0272-37fc-40cb-8dde-5397fdaeb88b.png',
          url: 'https://github.com/milkcat1994/SSAFYPJT_1'
        },
        {
          num: 2,
          img: 'https://user-images.githubusercontent.com/18321002/128350389-bbaae485-2774-4972-819a-4f38a2e2f451.png',
          url: 'https://github.com/milkcat1994/SSAFYPJT_2'
        },
        {
          num: 3,
          img: 'https://user-images.githubusercontent.com/18321002/128350391-5d291713-a6d2-45dd-be67-faa239b8a10e.png',
          url: 'https://github.com/milkcat1994/SSAFYPJT_3'
        }
      ]
    }
  },
  components: {
    ProjectCard
  }
}
</script>

<style lang="scss" scoped>
@import './main.scss';

</style>>
