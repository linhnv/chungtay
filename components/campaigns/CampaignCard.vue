<template>
  <div class="card">
    <div class="card-image">
      <figure class="image is-4by3">
        <img src="https://bulma.io/images/placeholders/1280x960.png" alt="Placeholder image">
      </figure>
    </div>
    <div class="card-content">
      <p class="title is-5">{{ title }}</p>
      <div class="content">
        {{ description }}
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

<style>
  .card-content{
    height: 188px;
    overflow: hidden;
  }
</style>