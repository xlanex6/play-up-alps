<template lang="pug">
  container.container
    app-logo
    h1.title
      | play-up-alps
    h2.subtitle
      | Play Up Alps website
    .links
      a.button--green(href='https://nuxtjs.org/', target='_blank') Documentation
      a.button--grey(href='https://github.com/nuxt/nuxt.js', target='_blank') GitHub

</template>

<script>
import AppLogo from '~/components/AppLogo.vue'

export default {
  components: {
    AppLogo
  }
}
</script>

<style lang="scss">
.container {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: $primary;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>

