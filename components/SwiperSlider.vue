<template>
  <div class="swiper-container">
      <div :style="`transform: translate3d(${translate}px, 0px, 0px);`" class="swiper-wrapper">   
          <div @mouseup="checkTranslate" class="swiper-slide">Slide 1 Slide 1 Slide 1 Slide 1 Slide 1 Slide 1 Slide 1Slide Slide 1 Slide 1 Slide 1 Slide 1 Slide 1 Slide 1 Slide 1Slide  Slide 1 Slide 1 Slide 1 Slide 1 Slide 1 Slide 1 Slide 1Slide  Slide 1 Slide 1 Slide 1 Slide 1 Slide 1 Slide 1 Slide 1Slide 1</div>    
      </div>
  </div>
</template>

<script>
import Swiper, { Thumbs } from 'swiper'
import 'swiper/swiper-bundle.css'

Swiper.use([ Thumbs ])

export default {
   data() {
      return {
        thumbsSwiper: null,
        translate: 300,
      };
    },
    methods:{
      checkTranslate(evt){
        console.log(evt)
      }
    },
    mounted() {
      new Swiper('.swiper-container', {
        scrollbar: {
          el: '.swiper-scrollbar',
          draggable: true,
        },
        
      })
    }
}
</script>

<style scoped>

</style>