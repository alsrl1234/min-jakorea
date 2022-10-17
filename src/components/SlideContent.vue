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
    <swiper-slide v-for="item in SlideData" :key="item">
      <div class="title_wrap">
        <div class="main_title" v-html="item.mainTitle"></div>
        <div class="sub_title">{{item.subtitle}}</div>
        <div class="slide_icon"><a href="">자세히보기<i class="fa-solid fa-arrow-right"></i></a></div>
      </div>
      <!-- <video :src="`./images/01mainSlide_video/${item.mVideo}`"></video> -->
    </swiper-slide>
  </swiper>
</template>
  <script>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from "swiper/vue";

// Import Swiper styles
import "swiper/css";

import "swiper/css/pagination";
import "swiper/css/navigation";

//   import "./style.css";

// import required modules
import { Autoplay, Pagination, Navigation } from "swiper";

export default {
  props:["SlideData"],
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
  
<style>
.swiper-slide {
  height: 750px;
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: #dfeff0;
}

.slide_icon{
  width: 215px;
  height: 65px;
  background-color: #fff;
  border-radius: 50px;
  
}
.slide_icon a{
  width: 100%;
  height: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
}

.main_title{
  font-size: 66px;
  color: #285F74;
}
.sub_title{
  font-size: 18px;
  color: #285F74;
}
</style>
  