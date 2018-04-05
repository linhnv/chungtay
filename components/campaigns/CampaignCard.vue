<template>
  <router-link :to="{ name: 'campaigns-id', params: { id: campaign.id }}">
    <div class="card">
      <div class="card-image">
        <figure class="image is-4by3">
          <img src="https://bulma.io/images/placeholders/1280x960.png" alt="Placeholder image">
        </figure>
      </div>
      <div class="card-content">
        <div class="card-content-wrapper">
          <p class="title is-5">{{ campaign.title }}</p>
          <div class="content">
            {{ campaign.description }}
          </div>
        </div>
      </div>
    </div>
  </router-link>
</template>

<script>
export default {
  name: 'CampaignCard',
  props: ['campaign'],
  data: function(){
    return {
    }
  }
}
</script>

<style scoped>
  /* TODO set only for tablet above*/
  .card-content-wrapper{
    height: 165px;
    overflow: hidden;
  }
</style>