<template>
  <div>
    <navbar/>
    <section class="hero is-primary">
      <div class="hero-body">
        <div class="container">
          <h1 class="title">
            Bulma.io  with Full Width Menu (Mega Menu)
          </h1>
          <h2 class="subtitle">
            Hover over Blog
          </h2>
        </div>
      </div>
    </section>
    <app-footer/>
  </div>
</template>

<script>
import Navbar from '~/components/Navbar.vue'
import AppFooter from '~/components/AppFooter.vue'

export default {
  components: {
    Navbar,
    AppFooter
  }
}
</script>

<style>
</style>
