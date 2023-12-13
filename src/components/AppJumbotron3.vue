<script>
  import { Swiper, SwiperSlide } from 'swiper/vue';

// Import Swiper styles
import 'swiper/css';

import 'swiper/css/pagination';

import '../styles/general.scss';

// import required modules
import { Pagination } from 'swiper/modules';

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    return {
      modules: [Pagination],
    };
  },
};
</script>

<template>
    
    <swiper :spaceBetween="30" :pagination="{clickable: true,}" :modules="modules" class="mySwiper">
    <swiper-slide>
        <div id="wrapperJumbo">
            <div class="icn">
                <img src="../../public/img/image (20).svg">
            </div>
            <div>
                <span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Nulla officia officiis est possimus. Dignissimos at possimus. Lorem ipsum dolor sit amet consectetur adipisicing elit. Deserunt quo commodi eos aut ratione repellat, consectetur quos libero quod facere ipsum explicabo ab optio repellendus odit similique atque! Est, provident?
                </span>
            </div>
            <div class="profilo">
                <img src="../../public/img/02.jpg">
                <div class="descr">
                    <h3>JOHN DOE</h3>
                    <span>deigner</span>
                </div>
            </div>
        </div>
    </swiper-slide>
    <swiper-slide><p>CIAO 2</p></swiper-slide>
    <swiper-slide>CIAO 3</swiper-slide>

<!-- <div class="positioning">    
    <div id="wrapperJumbo">
        <div class="icn">
           <img src="../../public/img/image (20).svg">
        </div>
        <div>
            <span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Nulla officia officiis est possimus. Dignissimos at possimus. Lorem ipsum dolor sit amet consectetur adipisicing elit. Deserunt quo commodi eos aut ratione repellat, consectetur quos libero quod facere ipsum explicabo ab optio repellendus odit similique atque! Est, provident?
            </span>
        </div>
        <div class="profilo">
            <img src="../../public/img/02.jpg">
            <div class="descr">
                <h3>JOHN DOE</h3>
                <span>deigner</span>
            </div>
        </div>
    </div>
</div> -->
</swiper>
</template>

<style scoped>
#wrapperJumbo{
    width: 60%;
    margin-left: auto;
    margin-right: auto;
    margin-top: 10%;
}
.mySwiper{
    min-height: 70vh;   
    background-image: url("../../public/img/Parallax-02.jpg");
    background-attachment: fixed;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
}
/* .positioning > img{
    width: 100%;
    height: 100%;
}
.positioning{
    height: 550px;
} */
.icn{
    width: 5%;
    filter: invert();
    margin-left: auto;
    margin-right: auto;
}
.profilo{
    display: flex;
    justify-content: center;
    margin-top: 2rem;
}
.desc{
    display: flex;
}
span , h3{
    color: white;
    margin-top: 0;
}

</style>