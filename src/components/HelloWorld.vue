<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p>
      Musicademadrid.es Nuevo frontend VUEJS - maquetación y componentes
    </p>
    
  </div>
</template>

<script lang="ts">
import Vue from 'vue';

export default Vue.extend({
  name: 'HelloWorld',
  props: {
    msg: String,
  }
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../scss/styles';

h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
  li {
    display: inline-block;
    margin: 0 10px;
  }
}
a {
  color: $button-primary-color;
}
</style>
