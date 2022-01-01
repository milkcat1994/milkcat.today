<template>
  <div id="header" class="top shadow-10">
    <div class="header-ui">
        <div class="name" v-on:click="moveMilkcatMain">
            Milkcat
        </div>

        <div class="git-img" v-on:click="moveMilkcatGitHub">
            <img class="profile" :src="require('@/assets/GitHub-Mark-32px.png')" alt="Github_url">
        </div>
        <div class="profile-img mr-10" v-on:click="moveAbout">
            <img class="profile" src="https://user-images.githubusercontent.com/18321002/115113251-57c70800-9fc4-11eb-928e-0767ede421c5.png" alt="Milkcat">
        </div>

    </div>
  </div>
</template>

<script>
export default {
  methods: {
    moveMilkcatGitHub: function () {
      window.open('https://github.com/milkcat1994', '_blank')
    },
    moveMilkcatMain: function () {
      this.$router.push('/')
    },
    moveAbout: function () {
      this.$router.push('about')
    }
  }
}
</script>

<style lang="scss" scoped>
@import './index.scss';

</style>>
