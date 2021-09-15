<template>
  <div :class="[componentClass, modify]">
      <a :href="enlace">
        <img :src="img" alt="">
      </a>
      <div class="c-song-square__text">
          <h3><a :href="enlace">{{ name }}</a></h3>
          <p>{{ genre }}</p>
      </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue';

export default Vue.extend({
  name: 'cSongSquare',
  props: {
    img: String,
    name: String,
    genre: String,
    modify: String,
    enlace: String
  },
  data() {
    return {      
      componentClass: 'c-song-square'
    }
  }
});
</script>
<style lang="scss" scoped>
@import '../scss/styles';
.c-song-square {
    text-align: left;
    margin-bottom: 10px;
    @media (min-width: $lg) {
        width: 50%;
    }

    img{
        width: 40%;
        height: auto;
        display: inline-block;
        vertical-align: top;
    }
    &__text {
        display: inline-block;
        vertical-align: top;
        padding-left: 16px;
        width: 50%;

        a {
            color: $white;
            text-decoration: none;
        }

        h3 {
            a {
                @media (min-width: $md) and (max-width: $max-md) {
                    font-size: 1rem;
                }
                font-size: 1.5rem;
            }
        }

        p {
            a {
                @media (min-width: $md) and (max-width: $max-md) {
                    font-size: 14px;
                }
                font-size: 1rem;
            }            
        }
    }
}
</style>