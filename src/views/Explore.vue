<template>
  <div class="explore animate__animated animate__fadeInUp" id="start">
    <img alt="Vue logo" class="logo-img" src="../assets/logo-no-font.svg">
    <div class="o-container">
      <div class="o-row">
        <div class="o-col-xs-12 u-pad-0">
          <c-search-input placeholder="BUSCA UN ARTISTA O GRUPO DE MADRID" />
        </div>
      </div>
      <div class="o-row">
        <div class="o-col-xs-12 u-pad-0 u-hidden-desk">
          <p class="u-xs-txt">Scrolla entre los géneros y filtra tu búsqueda</p>
        </div>
      </div>
      <div class="o-row genre-container">
          <c-genre-card href="#" modify="c-genre-card--w-25" img="https://musicademadrid.es/img/estilos/trap.png" alt="Trap" name="Trap" />
          <c-genre-card href="#" modify="c-genre-card--w-25" img="https://musicademadrid.es/img/estilos/trap.png" alt="Trap" name="Trap" />
          <c-genre-card href="#" modify="c-genre-card--w-25" img="https://musicademadrid.es/img/estilos/trap.png" alt="Trap" name="Trap" />
          <c-genre-card href="#" modify="c-genre-card--w-25" img="https://musicademadrid.es/img/estilos/trap.png" alt="Trap" name="Trap" />
          <c-genre-card href="#" modify="c-genre-card--w-25" img="https://musicademadrid.es/img/estilos/trap.png" alt="Trap" name="Trap" />
          <c-genre-card href="#" modify="c-genre-card--w-25" img="https://musicademadrid.es/img/estilos/trap.png" alt="Trap" name="Trap" />
          <c-genre-card href="#" modify="c-genre-card--w-25" img="https://musicademadrid.es/img/estilos/trap.png" alt="Trap" name="Trap" />
          <c-genre-card href="#" modify="c-genre-card--w-25" img="https://musicademadrid.es/img/estilos/trap.png" alt="Trap" name="Trap" />
          <c-genre-card href="#" modify="c-genre-card--w-25" img="https://musicademadrid.es/img/estilos/trap.png" alt="Trap" name="Trap" />
          <c-genre-card href="#" modify="c-genre-card--w-25" img="https://musicademadrid.es/img/estilos/trap.png" alt="Trap" name="Trap" />
          <c-genre-card href="#" modify="c-genre-card--w-25" img="https://musicademadrid.es/img/estilos/trap.png" alt="Trap" name="Trap" />
          <c-genre-card href="#" modify="c-genre-card--w-25" img="https://musicademadrid.es/img/estilos/trap.png" alt="Trap" name="Trap" />
          <c-genre-card href="#" modify="c-genre-card--w-25" img="https://musicademadrid.es/img/estilos/trap.png" alt="Trap" name="Trap" />
      </div>
    </div>
    <div class="o-container">          
      <cTitle title="Explora la música de Madrid" subtitle="" modify="c-title--left" />  
      <div class="o-row">
        <cSongSquare enlace="#" genre="Electrónica" img="https://musicademadrid.es/img/ira.jpg" name="Nombre del grupo musical" />
        <cSongSquare enlace="#" genre="Electrónica" img="https://musicademadrid.es/img/ira.jpg" name="Nombre del grupo musical" />
        <cSongSquare enlace="#" genre="Electrónica" img="https://musicademadrid.es/img/ira.jpg" name="Nombre del grupo musical" />
        <cSongSquare enlace="#" genre="Electrónica" img="https://musicademadrid.es/img/ira.jpg" name="Nombre del grupo musical" />
        <cSongSquare enlace="#" genre="Electrónica" img="https://musicademadrid.es/img/ira.jpg" name="Nombre del grupo musical" />
        <cSongSquare enlace="#" genre="Electrónica" img="https://musicademadrid.es/img/ira.jpg" name="Nombre del grupo musical" />
        <cSongSquare enlace="#" genre="Electrónica" img="https://musicademadrid.es/img/ira.jpg" name="Nombre del grupo musical" />
        <cSongSquare enlace="#" genre="Electrónica" img="https://musicademadrid.es/img/ira.jpg" name="Nombre del grupo musical" />
        <cSongSquare enlace="#" genre="Electrónica" img="https://musicademadrid.es/img/ira.jpg" name="Nombre del grupo musical" />
        <cSongSquare enlace="#" genre="Electrónica" img="https://musicademadrid.es/img/ira.jpg" name="Nombre del grupo musical" />
      </div>   
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import cTitle from '@/components/cTitle.vue';
import cSongSquare from '@/components/cSongSquare.vue';
import cSearchInput from '@/components/cSearchInput.vue';
import cGenreCard from '@/components/cGenreCard.vue';

export default {
  name: 'Explore',
  components: {
    cTitle,
    cSongSquare,
    cSearchInput,
    cGenreCard
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
.genre-container {
  @media (max-width: $max-sm) {
    height: 120px;
    overflow: scroll;
    border: 1px solid $button-primary-color;
    margin-top: 8px;
  }
}
</style>

