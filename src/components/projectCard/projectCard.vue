<template>
  <div class="project-card">
    <div class="card p-10">
      <div class="dp-inline-block project-card-left">
        <div class="border-b2"
        v-on:click="moveProjectGitHub">
          <img :src="require('@/assets/pjt/'+project.num+'.png')" class="card-img" alt="Project Thumbnail">
        </div>
        <span class="dp-block">
          {{project.name}}
        </span>
      </div>
      <div class ="dp-inline-block project-card-right">
        <span class=".dp-inline-block">
          {{project.info}}
        </span>
      </div>
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
