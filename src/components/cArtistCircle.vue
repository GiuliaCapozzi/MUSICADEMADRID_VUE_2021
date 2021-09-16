<template>
  <div :class="[componentClass, modify]">
      <div class="c-artist-circle__wrapper">
          <div class="c-artist-circle__img">
              <a :href="enlace"><img :src="img" :alt="alt" class="c-artist-circle__img-img"></a>
          </div>
          <div class="c-artist-circle__name">              
              <h3><a :href="enlace">{{ name }}</a></h3>
          </div>
      </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue';

export default Vue.extend({
  name: 'cArtistCircle',
  props: {
    img: String,
    alt: String,
    name: String,
    modify: String,
    enlace: String
  },
  data() {
    return {      
      componentClass: 'c-artist-circle',
      title: 'ir al perfil de artista'
    }
  }
});
</script>

<style lang="scss" scoped>
    @import '../scss/styles';

    .c-artist-circle {
        &--w-33 {
            width: 32%;
            max-width: 32%;            
            flex-basis: 32%;
        }
        &__wrapper {
            width: 100%;
            max-width: 100%;
        }
        &__img {
            @media (max-width: $max-sm) {
                width: 60px;
                height: 60px;
            }
            width: 200px;
            height: 200px;
            margin: 0 auto;

            .c-artist-circle__img-img {
                border-radius: 50%;
                height: 100%;
                border: 2px solid $button-primary-color;
            }
        }

        &__name {
            h3 {
                text-align: center;
                a {
                    font-size: 14px;
                    text-decoration: none;
                    @media (min-width: $md) {
                        font-size: 1rem;
                    }
                    &:hover {
                        color: $white;
                    }
                }
            }
        }
    }
</style>