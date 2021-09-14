<template>
  <div :class="[componentClass, modify]">
    <h1>{{ title }}</h1>
    <p class="c-hello__text">
      {{ subtitle }}
    </p>
    
  </div>
</template>

<script lang="ts">
import Vue from 'vue';

export default Vue.extend({
  name: 'cTitle',
  props: {
    title: String,
    subtitle: String,
    modify: String
  },
  data() {
    return {      
      componentClass: 'c-title'
    }
  }
});
</script>

<style lang="scss" scoped>
  @import '../scss/styles';
  .c-title {
    &--left {
      text-align: left;
    }
  }
</style>