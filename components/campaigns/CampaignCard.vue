<template>
  <div class="card">
    <div class="card-image">
      <figure class="image is-4by3">
        <img src="https://bulma.io/images/placeholders/1280x960.png" alt="Placeholder image">
      </figure>
    </div>
    <div class="card-content">
      <div class="card-content-wrapper">
        <p class="title is-5">{{ title }}</p>
        <div class="content">
          {{ description }}
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'CampaignCard',
  props: ['title', 'description'],
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