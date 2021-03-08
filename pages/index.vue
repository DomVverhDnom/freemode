<template>
  <div class="header">
     <div class="container">
        <div class="topWrapper">
            <div class="feedback">Обратная связь</div>
            <div class="logo">ЛОГО</div>
            <div class="number">89383402819</div>
          </div>
        <div class="botWrapper">
            <div class="funtions">заглушка</div>
          <div class="swiper-container">
              <div class="swiper-wrapper">   
                <div  class="swiper-slide">Slide 1 Slide 1 Slide 1 Slide 1 Slide 1 Slide 1 Slide 1Slide Slide 1 Slide 1 Slide 1 Slide 1 Slide 1 Slide 1 Slide 1Slide  Slide 1 Slide 1 Slide 1 Slide 1 Slide 1 Slide 1 Slide 1Slide  Slide 1 Slide 1 Slide 1 Slide 1 Slide 1 Slide 1 Slide 1Slide 1</div>    
              </div>
          </div>
            <div class="number">заглушка</div>
        </div>
    
     </div>
    </div>
</template>

<script>
import Swiper from 'swiper'
import 'swiper/swiper-bundle.css'

export default {
    mounted() {
      new Swiper('.swiper-container', {
        scrollbar: {
          el: '.swiper-scrollbar',
          draggable: true,
        },
        slidesPerView: 0.3,
        freeMode: true,
        
      })
    }
}
</script>

<style>
.container{
  max-width: 1280px;
  margin: 0 auto;
}
.topWrapper, 
.botWrapper {
  display: flex;
  justify-content: space-between;
  margin-top: 30px;
}
.swiper-container{ 
  max-width: 500px;
  cursor: pointer;
}



</style>
