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
    data() {
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

<template>
  <swiper
    :slides-per-view="1"
    :space-between="50"
    @swiper="onSwiper"
    @slideChange="onSlideChange"
  >
    <swiper-slide>
      <img src="../../public/img/Gallery-01.jpg">
    </swiper-slide>
    <swiper-slide>
      <img src="../../public/img/Gallery-02.jpg">
    </swiper-slide>
    <swiper-slide>Slider 3</swiper-slide>
    ...
  </swiper>
</template>

<style scoped>
.swiper {
  width: 600px;
  height: 300px;
}</style>