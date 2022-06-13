<template>
  <swiper
    :slides-per-view="3"
    :space-between="50"
    @swiper="onSwiper"
    @slideChange="onSlideChange"
    parallax
    :navigation="true"
    :slidesPerView="'auto'"
    :centeredSlides="true"
  >
    <swiper-slide v-for="image in images" :key="image" class="swiper__wrapper">
      <img :src="image.imageUrl" alt="" />
      <div class="swiper__wrapper-info">
        <div class="swiper__description">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Officiis unde
          labore facere tempore rem vitae nostrum dignissimos quibusdam
          perspiciatis repellendus.
        </div>
        <div>
          <a href="">Купить</a>
        </div>
      </div>
    </swiper-slide>
  </swiper>
</template>

<script>
import SwiperCore from "swiper";
import { Swiper, SwiperSlide } from "swiper/vue";
import "swiper/css";
import "swiper/css/navigation";
export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  data() {
    return {
      parallaxSwiperWidth: 0,
      images: [
        {
          id: 1,
          imageUrl: require("../../assets/imgs/game-page/Battlegrounds.jpg"),
        },
        {
          id: 2,
          imageUrl: require("../../assets/imgs/game-page/Battlegrounds.jpg"),
        },
        {
          id: 3,
          imageUrl: require("../../assets/imgs/game-page/Battlegrounds.jpg"),
        },
        {
          id: 4,
          imageUrl: require("../../assets/imgs/game-page/Battlegrounds.jpg"),
        },
      ],
    };
  },
  setup() {
    return {
      modules: [Navigation],
    };
  },
};
</script>

<style lang="scss" scoped>
.swiper__wrapper {
  display: block;
  width: 100%;
  height: 100%;
  border: 1px solid rgba(245, 245, 247, 0.12);
  border-radius: 10px;
  position: relative;
  & img {
    // width: 100%;
  }
}
.swiper__wrapper-info {
  position: absolute;
  top: 49px;
}
</style>