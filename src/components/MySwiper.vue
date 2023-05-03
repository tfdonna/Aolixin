<template>
  <swiper
    :slides-per-view="1"
    :space-between="50"
    autoplay=true
    @swiper="onSwiper"
    @slideChange="onSlideChange"
  >
    <swiper-slide class="slide"><img alt="Vue logo" src="../assets/logo.png" ></swiper-slide>
    <swiper-slide><img class="imgs" alt="Vue logo" src="../assets/production/workshop1.jpg" ></swiper-slide>
    <swiper-slide><img class="imgs" alt="Vue logo" src="../assets/production/workshop6.jpg" ></swiper-slide>
    <swiper-slide><img class="imgs" alt="Vue logo" src="../assets/production/workshop3.jpg" ></swiper-slide>
    <swiper-slide><img class="imgs" alt="Vue logo" src="../assets/production/workshop12.jpg" ></swiper-slide>
    <swiper-slide><img class="imgs" alt="Vue logo" src="../assets/production/working.jpg" ></swiper-slide>
  </swiper>
</template>
<script>
  // Import Swiper Vue.js components
  import { Swiper, SwiperSlide } from 'swiper/vue';

  // Import Swiper styles
  import 'swiper/css';

  export default {
    components: {
      Swiper,
      SwiperSlide,
    },
    setup() {
      const onSwiper = (swiper) => {
        console.log(swiper);
      };
      const onSlideChange = () => {
        console.log('slide change');
      };
      return {
        onSwiper,
        onSlideChange,
      };
    },
  };
</script>
<style lang="less" scoped>
.slide{
    width: 100%;
    img{
        width: 100%;
        height: 20%;
    }
}
</style>
