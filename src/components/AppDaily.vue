<script>
import { Swiper, SwiperSlide } from 'swiper/vue';
import 'swiper/css';
import 'swiper/css/pagination';
import 'swiper/css/navigation';
import '../styles/general.scss';
import { Pagination, Navigation } from 'swiper/modules';
import AppCard4 from "./AppCard4.vue";
import { store } from "../store.js"

export default {
    name:"AppDaily",
  components: {
    Swiper,
    SwiperSlide,
    AppCard4,
  },
  setup() {
    return {
        store,
      modules: [Pagination, Navigation],
    };
  },
};
</script>

<template>
    <div class="topDaily">
        <span>LATEST NEWS</span>
        <h1>ARTICULES UPDATED DAILY</h1>
        </div>
    <swiper ref="{swiperRef}" :slidesPerView="3" :centeredSlides="true" :spaceBetween="30" :loop="true" :pagination="{type: 'fraction',}" :navigation="true" :modules="modules" class="mySwiper">
        <swiper-slide>
        <div class="card">
            <div class="cardTop">
                <img src="../../public/img/blog01.jpg">
            </div>
            <div class="cardDescr">
                <span id="day">May 27 ,2022 By Admin</span>
                <h3>RECAP YOUR LATEST COMPANY EVENT</h3>
                <span>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Cumque nesciunt consectetur excepturi voluptate magnam temporibus reprehenderit quidem adipisci</span>
            </div>
        </div>   
    </swiper-slide>
    <swiper-slide>
        <div class="card">
            <div class="cardTop">
                <img src="../../public/img/blog02.jpg">
            </div>
            <div class="cardDescr">
                <span id="day">May 07 ,2022 By Admin</span>
                <h3>RECAP YOUR LATEST COMPANY EVENT</h3>
                <span>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Cumque nesciunt consectetur excepturi voluptate magnam temporibus reprehenderit quidem adipisci</span>
            </div>
        </div>  
    </swiper-slide>
    <swiper-slide>
        <div class="card">
            <div class="cardTop">
                <img src="../../public/img/blog03.jpg">
            </div>
            <div class="cardDescr">
                <span id="day">April 10 ,2022 By Admin</span>
                <h3>RECAP YOUR LATEST COMPANY EVENT</h3>
                <span>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Cumque nesciunt consectetur excepturi voluptate magnam temporibus reprehenderit quidem adipisci</span>
            </div>
        </div>  
    </swiper-slide>
    <swiper-slide>
        <div class="card">
            <div class="cardTop">
                <img src="../../public/img/blog04.jpg">
            </div>
            <div class="cardDescr">
                <span id="day">March 10 ,2022 By Admin</span>
                <h3>RECAP YOUR LATEST COMPANY EVENT</h3>
                <span>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Cumque nesciunt consectetur excepturi voluptate magnam temporibus reprehenderit quidem adipisci</span>
            </div>
        </div>  
    </swiper-slide>
    <swiper-slide>
        <div class="card">
            <div class="cardTop">
                <img src="../../public/img/blog05.jpg">
            </div>
            <div class="cardDescr">
                <span id="day">Febrary 14 ,2022 By Admin</span>
                <h3>RECAP YOUR LATEST COMPANY EVENT</h3>
                <span>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Cumque nesciunt consectetur excepturi voluptate magnam temporibus reprehenderit quidem adipisci</span>
            </div>
        </div>  
    </swiper-slide>
    <swiper-slide>
        <div class="card">
            <div class="cardTop">
                <img src="../../public/img/blog06.jpg">
            </div>
            <div class="cardDescr">
                <span id="day">December 07 ,2021 By Admin</span>
                <h3>RECAP YOUR LATEST COMPANY EVENT</h3>
                <span>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Cumque nesciunt consectetur excepturi voluptate magnam temporibus reprehenderit quidem adipisci</span>
            </div>
        </div>  
    </swiper-slide>
    <swiper-slide>
        <div class="card">
            <div class="cardTop">
                <img src="../../public/img/blog07.jpg">
            </div>
            <div class="cardDescr">
                <span id="day">December 22 ,2021 By Admin</span>
                <h3>RECAP YOUR LATEST COMPANY EVENT</h3>
                <span>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Cumque nesciunt consectetur excepturi voluptate magnam temporibus reprehenderit quidem adipisci</span>
            </div>
        </div>  
    </swiper-slide>
  </swiper>
  <p class="append-buttons"></p>
</template>

<style scoped>
.topDaily{
    text-align: center;
    margin-top: 3rem;
}
p{
    margin-top: 0.3rem;
    font-size: 50px;
}
.card{
 width: 450px;
 margin: 1rem;
 color: black;
}
img{
 width: 100%;
 object-fit: contain;
}
.mySwiper{
    margin: 2rem;
}
#day{
    color: slategray;
}
</style>