<template>
  <div class="home">
    <img alt="Vue logo" class="logo-img" src="../assets/logo-no-font.svg">

    <HelloWorld msg="Bienvenido al futuro de musicademadrid"/>
    <div class="o-container u-mt-2">          
      <cTitle title="Círculos home page artistas" subtitle="" modify="c-title--left" /> 
      <div class="o-row space-between"> 
        <div class="o-container">
          <cCarousel />
        </div>
      </div>      
    </div>
    <div class="o-container u-mt-2">           
      <cTitle title="Botones" subtitle="" modify="c-title--left" /> 
      <div class="o-row">
          <div class="o-col-xs-12 u-text-left"> 

            <cButton enlace="#" modify="c-button--primary" text="Primary button" />

            <cButton enlace="#" modify="c-button--secondary" text="Secondary button" />

            <cButton enlace="#" modify="c-button--success" text="Success button" />
          </div>
      </div>      
    </div>
    <div class="o-container u-mt-2">
      <cTitle title="Cuadrículas géneros y artistas" subtitle="" modify="c-title--left" /> 
      <div class="o-row u-flex-column-md">        
            
            <cSongSquare enlace="#" name="Cinco chicos que hacen música" genre="Rap/HipHop" img="https://musicademadrid.es/img/ira.jpg" />  
                
            <cSongSquare enlace="#" name="Cinco chicos que hacen música" genre="Rap/HipHop" img="https://musicademadrid.es/img/ira.jpg" />  
                
            <cSongSquare enlace="#" name="Cinco chicos que hacen música" genre="Rap/HipHop" img="https://musicademadrid.es/img/ira.jpg" />  
                
            <cSongSquare enlace="#" name="Cinco chicos que hacen música" genre="Rap/HipHop" img="https://musicademadrid.es/img/ira.jpg" />  
      </div>      
    </div>
    <div class="o-container">
      <div class="o-row">        
        <div class="o-col-xs-12 o-col-md-4 u-pad-0">
            <cGenreCard href="#" img="https://musicademadrid.es/img/estilos/trap.png" alt="Trap" name="Trap" />
        <cGenreCard href="#" img="https://musicademadrid.es/img/estilos/trap.png" alt="Trap" name="Trap" />
        <cGenreCard href="#" img="https://musicademadrid.es/img/estilos/trap.png" alt="Trap" name="Trap" />
        <cGenreCard href="#" img="https://musicademadrid.es/img/estilos/trap.png" alt="Trap" name="Trap" />
        <cGenreCard href="#" img="https://musicademadrid.es/img/estilos/trap.png" alt="Trap" name="Trap" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue';
import cTitle from '@/components/cTitle.vue';
import cButton from '@/components/cButton.vue';
import cSongSquare from '@/components/cSongSquare.vue';
import cCarousel from '@/components/cCarousel.vue';
import cGenreCard from '@/components/cGenreCard.vue';

export default {
  name: 'Home',
  components: {
    HelloWorld,
    cTitle,
    cButton,
    cSongSquare,
    cCarousel,
    cGenreCard
  }
}
</script>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Barlow:wght@300&family=Roboto+Mono:wght@200&family=Turret+Road:wght@300&display=swap');
@import '../scss/styles';

.logo-img {
  height: 200px;
}
</style>
