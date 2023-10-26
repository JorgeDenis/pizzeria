<template>
  <div class="home">
    <slider-pizza/>
    <video-presentacion/>
    <banner/>
  </div>
</template>

<script>

import Banner from '@/components/home/Banner.vue'
import SliderPizza from '@/components/home/SliderPizza.vue';
import VideoPresentacion from '@/components/home/VideoPresentacion.vue';
export default {
  name: 'HomeView',
  components: {
    Banner,
    SliderPizza,
    VideoPresentacion
}
}
</script>
