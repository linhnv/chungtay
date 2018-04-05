<template>
  <div>
    <navbar/>
    <nuxt/>
    <app-footer/>
  </div>
</template>

<script>
import Navbar from '~/components/shared/Navbar.vue'
import AppFooter from '~/components/shared/AppFooter.vue'

export default {
  components: {
    Navbar,
    AppFooter,
  }
}
</script>

<style>
</style>
