<template>
  <a :href="href" :class="[componentClass, modify]">
      <i class="fas fa-play"></i> {{ text }}
  </a>
</template>

<script lang="ts">
import Vue from 'vue';

export default Vue.extend({
  name: 'cMusicListCard',
  props: {
    modify: String,
    text: String,
    href: String
  },
  data() {
    return {      
      componentClass: 'c-music-list-card'
    }
  }
});
</script>

<style lang="scss" scoped>
    @import url('https://fonts.googleapis.com/css2?family=Barlow:wght@300&family=Roboto+Mono:wght@200&family=Turret+Road:wght@300&display=swap');
    @import '../scss/styles';
  .c-music-list-card {
      display: block;
      width: 100%;
      text-align: left;
      font-size: 1.5rem;
      background-color: $bg-secondary;
      color: $white;
      border-bottom: 1px solid $white;
      padding: 20px;
      text-decoration: none;
      transition: all .3s ease-in-out;

      &:hover {
          box-shadow: $shadow-1;
      }
  }
</style>