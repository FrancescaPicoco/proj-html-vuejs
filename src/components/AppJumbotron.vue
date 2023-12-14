<script>
import { Swiper, SwiperSlide } from 'swiper/vue';
import 'swiper/css';
import 'swiper/css/pagination';
import 'swiper/css/navigation';
import '../styles/general.scss';
import { Autoplay, Pagination, Navigation } from 'swiper/modules';

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    return {
      modules: [Autoplay, Pagination, Navigation],
    };
  },
};
</script>

<template>
  <swiper
    :spaceBetween="30"
    :centeredSlides="true"
    :autoplay="{
      delay: 2500,
      disableOnInteraction: false,
    }"
    :pagination="{
      clickable: true,
    }"
    :navigation="true"
    :modules="modules"
    class="mySwiper"
  >
    <swiper-slide>
      <img src="../../public/img/Parallax-02.jpg">
      
    </swiper-slide>
    <swiper-slide>
      <img src="../../public/img/Parallax-03.jpg">
    </swiper-slide>
    <div class="cs">
      <span>CINEMA STUDIO</span>
      <p>ACTION AND INSPIRE PEOPLE</p>
      <button>READ MORE</button>
    </div>
  </swiper>
</template>

<style scoped>
.mySwiper{
  position: relative;
}
.cs{
  position: absolute;
  top: 0;
}

</style>