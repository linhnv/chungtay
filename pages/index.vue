<template>
  <div>
    <section class="hero is-primary is-medium">
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
          <div v-for="campaign in campaigns" :key="campaign.id" class="column">
            <campaign-card :campaign="campaign"/>
          </div>
        </div>
      </div>
    </section>
    <section class="section">
      <div class="container">
        <h2 class="title">News</h2>
        <div class="columns">
          <div v-for="campaign in campaigns" :key="campaign.id" class="column">
            <campaign-card :campaign="campaign"/>
          </div>
        </div>
      </div>
    </section>
    <section class="section">
      <div class="container">
        <app-statistics/>
      </div>
    </section>
  </div>
</template>

<script>
import AppStatistics from '~/components/homepage/AppStatistics.vue'
import CampaignCard from '~/components/campaigns/CampaignCard.vue'

export default {
  components: {
    CampaignCard,
    AppStatistics
  },
  data: function(){
    return {
      campaigns: [
        {
          id: 1,
          title: 'Lorem ipsum dolor sit amet',
          description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus nec iaculis mauris.'
        },
        {
          id: 2,
          title: 'Lorem ipsum dolor sit amet consectetur',
          description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus nec iaculis mauris.'
        },
        {
          id: 3,
          title: 'Lorem ipsum dolor siet',
          description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus nec iaculis mauris.'
        },
        {
          id: 4,
          title: 'Lorem ipsum dolor sit amet',
          description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. '
        },
      ]
    }
  }
}
</script>

