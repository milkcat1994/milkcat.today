<template>
  <div id="main">
      <Dividor title="Project" />
      <ProjectCard v-for="(project, key) in projects" v-bind:key="key"
      v-bind:pjt="project"
      />
  </div>
</template>

<script>
import ProjectCard from '@/components/projectCard/projectCard.vue'
import Dividor from '@/components/main/dividor/dividor.vue'

export default {
  data () {
    return {
      projects: [
        {
          num: 1,
          name: '편집',
          img: 'https://user-images.githubusercontent.com/18321002/128350386-a12e0272-37fc-40cb-8dde-5397fdaeb88b.png',
          url: 'https://github.com/milkcat1994/SSAFYPJT_1',
          info: '편집자와의 매칭 사이트 입니다.'
        },
        {
          num: 2,
          name: '푸드 메이트',
          img: 'https://user-images.githubusercontent.com/18321002/128350389-bbaae485-2774-4972-819a-4f38a2e2f451.png',
          url: 'https://github.com/milkcat1994/SSAFYPJT_2',
          info: '음식 궁합 검색 및 식단 기록 애플리케이션 입니다.'
        },
        {
          num: 3,
          name: 'Face OFF',
          img: 'https://user-images.githubusercontent.com/18321002/128350391-5d291713-a6d2-45dd-be67-faa239b8a10e.png',
          url: 'https://github.com/milkcat1994/SSAFYPJT_3',
          info: '자동 사진 모자이크 웹 애플리케이션 입니다.'
        }
      ]
    }
  },
  components: {
    ProjectCard,
    Dividor
  }
}
</script>

<style lang="scss" scoped>
@import './main.scss';

</style>>
