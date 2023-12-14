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
    :slidesPerView="4"
    :loop="true"
    :spaceBetween="30"
    :centeredSlides="true"
    :autoplay="{
      delay: 2500,
      disableOnInteraction: false,
    }"
    :pagination="{
      type: 'fraction',
    }"
    :navigation="true"
    :modules="modules"
    class="mySwiper"
  >
    <swiper-slide>
        <img src="../../public/img/01.png">
    </swiper-slide>
    <swiper-slide>
        <img src="../../public/img/02.png">
    </swiper-slide>
    <swiper-slide>
        <img src="../../public/img/03.png">
    </swiper-slide>
    <swiper-slide>
        <img src="../../public/img/04.png">
    </swiper-slide>
    <swiper-slide>
        <img src="../../public/img/05.png">
    </swiper-slide>
  </swiper>
</template>

<style scoped>
.mySwiper{
    height: 40vh;
    background-image: url("../../public/img/Parallax-03.jpg");
    min-height: 30vh;
    background-attachment: fixed;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    margin-top: 3rem;
}
img{
  margin-top: 27%;
}
</style>