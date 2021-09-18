<template>
  <div class="dp-block card p-10">
    <div class="border-b2"
    v-on:click="moveProjectGitHub">
      <img :src="require('@/assets/pjt/'+project.num+'.png')" class="card-img" alt="">
    </div>
  </div>
</template>

<script>
export default {
  props: [
    'pjt'
  ],
  data () {
    return {
      project: this.pjt
    }
  },
  methods: {
    moveProjectGitHub: function () {
      window.open(this.project.url)
    }
  }
}
</script>

<style lang="scss" scoped>
@import './projectCard.scss';

</style>
