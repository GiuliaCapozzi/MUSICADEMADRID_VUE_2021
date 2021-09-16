<template>
  <a :href="href" :class="[componentClass, modify]">
      <div class="c-genre-card__wrapper">
          <img :src="img" :alt="alt">
          <h3>{{ name }}</h3>
      </div>
  </a>
</template>

<script lang="ts">
import Vue from 'vue';

export default Vue.extend({
  name: 'cGenreCard',
  props: {
    name: String,
    img: String,
    alt: String,
    href: String,
    modify: String
  },
  data() {
    return {      
      componentClass: 'c-genre-card'
    }
  }
});
</script>

<style lang="scss" scoped>
    @import url('https://fonts.googleapis.com/css2?family=Barlow:wght@300&family=Roboto+Mono:wght@200&family=Turret+Road:wght@300&display=swap');
    @import '../scss/styles';
    .c-genre-card {
        text-align: left;
        background-color: $bg-secondary;
        display: inline-block;
        margin: 10px 0;
        transition: all .3s ease-in-out;
        @media (max-width: $max-sm) {
          width: 45%;
          text-align: center;
          margin: 8px;
          display: inline-block;
          line-height: 6px;
        }

        img {
            @media (max-width: $max-sm) {
              width: 60px;
              height: 60px;
            }

            width: 30%;
            display: inline-block;
        }

        h3 {
            display: inline-block;
            width: 70%;
            font-size: 1.5rem;
        }

        &:hover {
            box-shadow: $shadow-1;
        }

        &--w-25 {
          h3{
            font-size: .8rem;
          }
          @media (min-width: $md) {
            width: 10%;
            flex-basis: 10%;
            max-width: 10%;
            margin-right: 8px;
          }
        }
    }
</style>