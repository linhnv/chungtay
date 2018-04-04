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
    <section class="section">
      <div class="container">
        <h2 class="title">Trending campaigns</h2>
        <div class="columns">
          <div class="column">
            <campaign-card
              :title="'Lorem ipsum dolor sit amet'"
              :description="'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus nec iaculis mauris.'"
            />
          </div>
          <div class="column">
            <campaign-card
              :title="'Lorem ipsum dolor sit amet, consectetur adipiscing elit'"
              :description="'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus nec iaculis mauris.'"
            />
          </div>
          <div class="column">
            <campaign-card
              :title="'Lorem ipsum dolor sit amet'"
              :description="'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus nec iaculis mauris.'"
            />
          </div>
          <div class="column">
            <campaign-card
              :title="'Lorem ipsum dolor sit amet'"
              :description="'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus nec iaculis mauris.'"
            />
          </div>
        </div>
      </div>
    </section>
    <section class="section">
      <div class="container">
        <h2 class="title">News</h2>
        <div class="columns">
          <div class="column">
            <campaign-card
              :title="'Lorem ipsum dolor sit amet'"
              :description="'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus nec iaculis mauris.'"
            />
          </div>
          <div class="column">
            <campaign-card
              :title="'Lorem ipsum dolor sit amet, consectetur adipiscing elit'"
              :description="'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus nec iaculis mauris.'"
            />
          </div>
          <div class="column">
            <campaign-card
              :title="'Lorem ipsum dolor sit amet'"
              :description="'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus nec iaculis mauris.'"
            />
          </div>
          <div class="column">
            <campaign-card
              :title="'Lorem ipsum dolor sit amet'"
              :description="'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus nec iaculis mauris.'"
            />
          </div>
        </div>
      </div>
    </section>
    <section class="section">
      <div class="container">
        <app-statistics/>
      </div>
    </section>
    <app-footer/>
  </div>
</template>

<script>
import Navbar from '~/components/Navbar.vue'
import AppFooter from '~/components/AppFooter.vue'
import AppStatistics from '~/components/AppStatistics.vue'
import CampaignCard from '~/components/campaigns/CampaignCard.vue'

export default {
  components: {
    Navbar,
    AppFooter,
    CampaignCard,
    AppStatistics
  }
}
</script>

