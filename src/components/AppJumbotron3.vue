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
                <span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Nulla officia officiis est possimus. consectetur adipisicing elit. Deserunt quo commodi eos aut ratione repellat, consectetur quos libero quod facere ipsum explicabo ab optio repellendus odit similique atque! Est, provident?
                </span>
            </div>
            <div class="profilo">
                <div class="img">
                    <img src="../../public/img/03.jpg">
                </div>
                <div class="descr">
                    <p>JOHN DOE</p>
                    <span>deigner</span>
                </div>
            </div>
        </div>
    </swiper-slide>
    <swiper-slide>
        <div id="wrapperJumbo">
            <div class="icn">
                <img src="../../public/img/image (20).svg">
            </div>
            <div>
                <span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Nulla officia officiis est possimus. consectetur adipisicing elit. Deserunt quo commodi eos aut ratione repellat, consectetur quos libero quod facere ipsum explicabo ab optio repellendus odit similique atque! Est, provident?
                </span>
            </div>
            <div class="profilo">
                <div class="img">
                    <img src="../../public/img/02.jpg">
                </div>
                <div class="descr">
                    <p>JOHN DOE</p>
                    <span>deigner</span>
                </div>
            </div>
        </div>
    </swiper-slide>
    <swiper-slide>
        <div id="wrapperJumbo">
            <div class="icn">
                <img src="../../public/img/image (20).svg">
            </div>
            <div>
                <span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Nulla officia officiis est possimus. consectetur adipisicing elit. Deserunt quo commodi eos aut ratione repellat, consectetur quos libero quod facere ipsum explicabo ab optio repellendus odit similique atque! Est, provident?
                </span>
            </div>
            <div class="profilo">
                <div class="img">
                    <img src="../../public/img/03.jpg">
                </div>
                <div class="descr">
                    <p>JOHN DOE</p>
                    <span>deigner</span>
                </div>
            </div>
        </div>
    </swiper-slide>
</swiper>
</template>

<style scoped>
#wrapperJumbo{
    width: 50%;
    margin-left: auto;
    margin-right: auto;
    margin-top: 15%;
    line-height: 2;
}
.mySwiper{
    min-height: 90vh;   
    background-image: url("../../public/img/Parallax-02.jpg");
    background-attachment: fixed;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
}
.img > img{
    border-radius: 50px;
    width: 60px;
    margin: 1rem;
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
span , p{
    color: white;
    text-align: center;
}

</style>