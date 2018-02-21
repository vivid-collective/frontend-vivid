<template>
  <div id="app">
    <v-app>
      <navigation></navigation>
      <router-view/>
    </v-app>
  </div>
</template>

<script>

import navigation from './components/Navigation.vue'
import landingPage from './components/LandingPage.vue'

export default {
  name: 'App',
  components: {
    navigation,
    landingPage
  }
}
</script>

<style>

</style>
