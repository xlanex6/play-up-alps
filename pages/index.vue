<template lang="pug">
  section.has-bg-img
    .container
      img.bubble(src="~assets/bubble.png")
      .pua-navbar
        img.logo(src="~assets/logo.png")
      .pua-header
        h1 test
        img(src="~assets/logo-title.png")
    

        //- .pua-highlight Activer et rassembler l’arc alpin pour contribuer au développement de réussites
</template>

<script>
import AppLogo from "~/components/AppLogo.vue";

export default {
  components: {
    AppLogo
  }
};
</script>

<style lang="stylus">
.pua-highlight
  background: $primary
  color: $white
  letter-spacing: 0.64px
  line-height: 25px
.pua-navbar
  img.logo
    height 35px
    width 50px
    margin-top 30px
.pua-header
  position relative
  display flex
  align-items center
  justify-content center
img.bubble 
  position absolute
  width 632px
  height 507px
  top 150px
  right -37px



  img 
    width 100px
.has-bg-img
  height 640px
  background url("/assets/header-bg.jpg") center center
  background-size cover
  
</style>

