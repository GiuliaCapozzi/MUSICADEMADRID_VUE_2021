<template>
  <div class="home animate__animated animate__fadeIn" id="start">
    <img alt="Vue logo" class="logo-img" src="../assets/logo-no-font.svg">
    <div class="o-container u-mt-2">          
      <cTitle title="Artistas de Madrid" subtitle="" modify="c-title--left" /> 
      <div class="o-row space-between"> 
        <div class="o-container">
          <cCarousel />
        </div>
      <div class="btn-container">
        <cButton isRouter="true" enlace="/explora" modify="c-button--primary" text="Ver todos lo artistas de Madrid" />
      </div>
      </div>      
    </div>
    <div class="o-container u-add-mt">         
      <cTitle title="Géneros musicales en Madrid" subtitle="" modify="c-title--left" /> 
      <div class="o-row">        
        <div class="o-col-xs-12 o-col-md-4 u-pad-0">
            <cGenreCard href="#" img="https://musicademadrid.es/img/estilos/trap.png" alt="Trap" name="Trap" />
            <cGenreCard href="#" img="https://musicademadrid.es/img/estilos/trap.png" alt="Trap" name="Trap" />
            <cGenreCard href="#" img="https://musicademadrid.es/img/estilos/trap.png" alt="Trap" name="Trap" />
            <cGenreCard href="#" img="https://musicademadrid.es/img/estilos/trap.png" alt="Trap" name="Trap" />
            <cGenreCard href="#" img="https://musicademadrid.es/img/estilos/trap.png" alt="Trap" name="Trap" />
        </div>
        <div class="o-col-xs-12 o-col-md-9 u-mt-10 u-pad-0-sm">
          <cSearchInput placeholder="BUSCA UN ARTISTA O GRUPO" />
          <cButton enlace="#" modify="c-button--secondary u-m-0 u-mt-10 c-button--w-100" text="Ver Artistas Trap" />
          
          <cMusicListCard href="#" text="Título de una canción" />
          <cMusicListCard href="#" text="Título de una canción" />
          <cMusicListCard href="#" text="Título de una canción" />
          <cMusicListCard href="#" text="Título de una canción" />
          <cMusicListCard href="#" text="Título de una canción" />
          <cMusicListCard href="#" text="Título de una canción" />
          <cMusicListCard href="#" text="Título de una canción" />
          <cMusicListCard href="#" text="Título de una canción" />
          <cMusicListCard href="#" text="Título de una canción" />
          <cMusicListCard href="#" text="Título de una canción" />

        </div>
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import cTitle from '@/components/cTitle.vue';
import cButton from '@/components/cButton.vue';
import cCarousel from '@/components/cCarousel.vue';
import cGenreCard from '@/components/cGenreCard.vue';
import cSearchInput from '@/components/cSearchInput.vue';
import cMusicListCard from '@/components/cMusicListCard.vue';

export default {
  name: 'Home',
  components: {
    cTitle,
    cButton,
    cCarousel,
    cGenreCard,
    cSearchInput,
    cMusicListCard
  }
}
</script>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Barlow:wght@300&family=Roboto+Mono:wght@200&family=Turret+Road:wght@300&display=swap');
@import '../scss/styles';
* {
  text-align: left;
}
.logo-img {
  height: 200px;
}
.btn-container {
  width: 100%;
  text-align: center;
  @media (min-width: $md) {
    text-align: right;
  }
}
</style>
