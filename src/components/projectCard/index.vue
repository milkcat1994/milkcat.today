<template>
  <div class="dp-block card p-10">
    <div class="border-b2"
    v-on:click="moveProjectGitHub">
      <!-- <img v-bind:src="project.img" class="card-img"> -->
      <img :src="require('@/assets/pjt/'+project.num+'.png')" class="card-img">
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
  },
  created () {
  }
}
</script>

<style lang="scss" scoped>
@import './index.scss';

</style>>
