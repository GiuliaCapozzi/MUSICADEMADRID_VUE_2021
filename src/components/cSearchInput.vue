<template>
  <input :placeholder="placeholder" type="text" :class="[componentClass, modify]">
</template>

<script lang="ts">
import Vue from 'vue';

export default Vue.extend({
  name: 'cSearchInput',
  props: {
    text: String,
    placeholder: String
  },
  data() {
    return {      
      componentClass: 'c-search-input'
    }
  }
});
</script>
<style lang="scss" scoped>
    @import url('https://fonts.googleapis.com/css2?family=Barlow:wght@300&family=Roboto+Mono:wght@200&family=Turret+Road:wght@300&display=swap');
    @import '../scss/styles';
    .c-search-input {
        background-color: $bg-secondary;
        border: none;
        color: $white;
        width: 100%;
    }
</style>