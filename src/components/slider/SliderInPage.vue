<template>
  <swiper
    :slides-per-view="3"
    :space-between="50"
    @swiper="onSwiper"
    @slideChange="onSlideChange"
    parallax
    grabCursor
    :navigation="true"
  >
    <swiper-slide v-for="image in images" :key="image" class="swiper__wrapper">
      <a href="/">
        <img :src="image.imageUrl" alt="" />
        <div class="swiper__wrapper-info">
          <h2>CS GO CS GO</h2>
          <p>MMO RPG</p>
        </div>
      </a>
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
  margin: 0 7px;
  border: 1px solid rgba(0, 0, 0, 0.1);
  width: 204px;
  height: 335px;
  & img {
    border-radius: 8px;
    width: 100%;
  }
}
.swiper__wrapper-info {
  position: absolute;
  bottom: -7px;
  width: 100%;
  background-color: rgba(50, 50, 54, 0.97);
  padding: 25px 14px;
  box-sizing: border-box;
  border-bottom-right-radius: 8px;
  border-bottom-left-radius: 8px;
  & h2 {
    font-size: 16px;
    line-height: 20px;
    text-decoration: none;
    color: #fff;
    transform: translateY(-11px);
  }
  & p {
    font-size: 13px;
    margin: 0;
    color: #979797;
    transform: translateY(-12px);
  }
}
@media (max-width: 1202px) {
}
</style>