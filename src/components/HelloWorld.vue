<template>
  <div class="c-hello">
    <h1>{{ msg }}</h1>
    <p class="c-hello__text">
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

.c-hello {  
  background-color: $bg-secondary;
  margin: 15px;
  @media (min-width: $md) {    
    width: 50%;
    margin: 0 auto;
  }
  box-shadow: $shadow-1;
  border-radius: 4px;
  padding: 20px;

  h1 {
    font-size: 1rem;
    @media (min-width: $md) {
      font-size: 2rem;
    }
  }

  p {
    font-size: 14px;
    @media (min-width: $md) {
      font-size: 1rem;
    }
  }

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
}
</style>
