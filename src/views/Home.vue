<template>
  <div class="home">
    <img alt="Vue logo" class="logo-img" src="../assets/logo-no-font.svg">

    <HelloWorld msg="Bienvenido al futuro de musicademadrid"/>
    <div class="o-container u-mt-2">          
      <cTitle title="Círculos home page artistas" subtitle="" modify="c-title--left" /> 
      <div class="o-row space-between"> 
        <cArtistCircle img="https://musicademadrid.es/img/ybeef.jpg" alt="Yung Beef" name="Yung Beef" modify="c-artist-circle--w-33" link="https://google.com" />
            
        <cArtistCircle img="https://musicademadrid.es/img/ybeef.jpg" alt="Yung Beef" name="Cinco chicos que hacen música" modify="c-artist-circle--w-33" link="https://google.com" />
            
        <cArtistCircle img="https://musicademadrid.es/img/ybeef.jpg" alt="Yung Beef" name="C. Tangana" modify="c-artist-circle--w-33" link="https://google.com" />
      </div>      
    </div>
    <div class="o-container u-mt-2">           
      <cTitle title="Botones" subtitle="" modify="c-title--left" /> 
      <div class="o-row">
          <div class="o-col-xs-12 u-text-left"> 

            <cButton modify="c-button--primary" text="Primary button" />

            <cButton modify="c-button--secondary" text="Secondary button" />

            <cButton modify="c-button--success" text="Success button" />
          </div>
      </div>      
    </div>
    <div class="o-container u-mt-2">
      <div class="o-row">
          <div class="o-col-xs-12">            
            <cTitle title="Cuadrículas géneros y artistas" subtitle="" modify="c-title--left" /> 
          </div>
      </div>      
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue';
import cTitle from '@/components/cTitle.vue';
import cArtistCircle from '@/components/cArtistCircle.vue';
import cButton from '@/components/cButton.vue';

export default {
  name: 'Home',
  components: {
    HelloWorld,
    cTitle,
    cArtistCircle,
    cButton
  }
}
</script>

<style lang="scss" scoped>
@import '../scss/styles';

.logo-img {
  height: 200px;
}
</style>
