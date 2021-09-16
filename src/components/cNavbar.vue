<template>
  <div :class="[componentClass, modify]">
      <nav class="c-navbar__wrapper" role="navigation">
          <ul>
              <li v-for="item of menuElements" :key="item.id">
                <router-link :to="item.link" :title="item.name">
                    <i :class="item.icon"></i>
                    <span class="c-navbar__mbl-text">
                        {{ item.name }}
                    </span>
                </router-link>
              </li>
          </ul>
      </nav>
  </div>
</template>

<script lang="ts">
import Vue from 'vue';

export default Vue.extend({
  name: 'cNavbar',
  props: {
      modify: String
  },
  data() {
    return {      
      componentClass: 'c-navbar',
      menuElements: [
          {
            name: 'Home',
            icon: 'fas fa-home',
            link: '/'
          },
          {
            name: 'Explora',
            icon: 'fas fa-search',
            link: '/explora'
          },
          {
            name: 'Escucha',
            icon: 'fas fa-headphones',
            link: '#'
          },
          {
            name: 'Agrega',
            icon: 'fas fa-plus',
            link: '#'
          }
      ]
    }
  }
});
</script>
<style lang="scss" scoped>  
    @import url('https://fonts.googleapis.com/css2?family=Barlow:wght@300&family=Roboto+Mono:wght@200&family=Turret+Road:wght@300&display=swap');
    @import '../scss/styles';
    .c-navbar {
        margin-top: 100px;
        &__wrapper {            
            background-color: $bg-secondary;
            height: 80px;
            display: block;
            position: fixed;
            bottom: 0;
            width: 100%;
        }
        ul {
            display: flex;
            justify-content: space-between;
            padding: 0 10%;
            li {
                line-height: 80px;
                a i{
                    font-size: 2rem;    
                    display: inline-block;
                    vertical-align: middle;
                    padding-right: 1rem;
                }
            }
        }

        &__mbl-text {
            display: inline-block;
            @media (max-width: $max-sm) {
                display: none;
            }
        }
    }
</style>