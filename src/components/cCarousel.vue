<template>
  <div :class="[componentClass, modify]">      
        <carousel :navigationEnabled="true" :paginationColor="'#fff'" :navigationClickTargetSize="0" :paginationEnabled="false" :perPageCustom="[[200, 3], [768, 3], [1024, 3]]" :autoplay="true" :autoplayTimeout="3000" :autoplayHoverPause="false" :centerMode="true" :loop="true">

            <slide>            
                 <cArtistCircle enlace="#" img="https://musicademadrid.es/img/ybeef.jpg" alt="Yung Beef" name="C. Tangana" link="https://google.com" />
            </slide>
            <slide>      
                 <cArtistCircle enlace="#" img="https://musicademadrid.es/img/ybeef.jpg" alt="Yung Beef" name="C. Tangana" link="https://google.com" />
            </slide>
            <slide>      
                 <cArtistCircle enlace="#" img="https://musicademadrid.es/img/ybeef.jpg" alt="Yung Beef" name="C. Tangana" link="https://google.com" />
            </slide>
            <slide>      
                 <cArtistCircle enlace="#" img="https://musicademadrid.es/img/ybeef.jpg" alt="Yung Beef" name="C. Tangana" link="https://google.com" />
            </slide>
            <slide>      
                 <cArtistCircle enlace="#" img="https://musicademadrid.es/img/ybeef.jpg" alt="Yung Beef" name="C. Tangana" link="https://google.com" />
            </slide>
            <slide>      
                 <cArtistCircle enlace="#" img="https://musicademadrid.es/img/ybeef.jpg" alt="Yung Beef" name="C. Tangana" link="https://google.com" />
            </slide>
            <slide>      
                 <cArtistCircle enlace="#" img="https://musicademadrid.es/img/ybeef.jpg" alt="Yung Beef" name="C. Tangana" link="https://google.com" />
            </slide>

        </carousel>
  </div>
</template>

<script lang="ts">
import Vue from 'vue';
import cArtistCircle from '@/components/cArtistCircle.vue';
import { Carousel, Slide } from 'vue-carousel';


export default Vue.extend({
  name: 'cCarousel',
  props: {
    img: String
  },
  components: {
    cArtistCircle,
    Carousel,
    Slide
  },
  data() {
    return {      
      componentClass: 'c-carousel'
    }
  }
});
</script>