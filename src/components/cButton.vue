<template>
  
  <router-link v-if="isRouter" :to="enlace" :class="[componentClass, modify]">
      {{ text }}
  </router-link>
  <a v-else :href="enlace" :class="[componentClass, modify]">
      {{ text }}
  </a>
</template>

<script lang="ts">
import Vue from 'vue';

export default Vue.extend({
  name: 'cButton',
  props: {
    text: String,
    modify: String,
    enlace: String,
    isRouter: Boolean
  },
  data() {
    return {      
      componentClass: 'c-button'
    }
  }
});
</script>

<style lang="scss" scoped>
@import '../scss/styles';
.c-button {
    text-transform: uppercase;
    margin: 5px;
    display: inline-block;
    font-weight: 400;
    text-align: center;
    white-space: nowrap;
    vertical-align: middle;
    user-select: none;
    border: 1px solid transparent;
    padding: .375rem .75rem;
    font-size: 1rem;
    line-height: 1.5;
    transition: all .15s ease-in-out,background-color .15s ease-in-out,border-color .15s ease-in-out,box-shadow .15s ease-in-out;

    &:hover {
        box-shadow: $shadow-1;
    }
    
    &--primary {
        background-color: $button-primary-color;
        color: $white;
        text-decoration: none;
    }
    
    &--secondary {
        background-color: $button-secondary-color;
        color: $white;
        text-decoration: none;
    }
    
    &--success {
        background-color: $success-green;
        color: $white;
        text-decoration: none;
    }

    &--w-100 {
      width: 100%;
    }
}
</style>