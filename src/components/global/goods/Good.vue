<template>
  <RouterLink to="/goods-page">
    <div>
      <div class="recommendations__picture">
        <img
          src="https://store.my.games/pre_240x145_crop/hotbox/showcase/gamelocaledraft/picture/56612309-e0b1-4254-8f5a-d98d6423d320.jpg"
          alt="Tom Clancy's Rainbow Six Siege онлайн" width="240" height="145" />
      </div>
      <div class="product__info-special sale">
        <span>-{{ item.sale }}%</span>
      </div>
      <div class="product__info-special price">
        <span>{{ item.price }}₽</span>
      </div>
    </div>
    <div class="recommendations__info">
      <div class="recommendations__info-top">
        <div class="recommendations__info-title">{{ item.title }}</div>
        <div class="recommendations__info-genre">{{ item.genre }}</div>
      </div>
      <div class="recommendations__info-descr">
        {{ item.description }}
      </div>
      <div class="recommendations__info-button">
        <div>Купить</div>
      </div>
    </div>
  </RouterLink>
</template>

<script>
import ButtonShowMore from "@/components/index/buttons/ButtonShowMore";

export default {
  components: {
    ButtonShowMore,
  },

  props: {
    item: {
      required: true,
      type: Object
    }
  },

  data() {
    return {
      items: [
        {
          title: "RAINBOWSIX SIEGE",
          sale: 80,
          price: 7990,
          genre: "Шутер",
          description:
            "Экшн-шутер в жанре зомби-апокалипсиса и с элементами строительства базы. Начните свой путь!",
        },
        {
          title: "RAINBOWSIX SIEGE",
          sale: 80,
          price: 7990,
          genre: "Шутер",
          description:
            "Экшн-шутер в жанре зомби-апокалипсиса и с элементами строительства базы. Начните свой путь!",
        },
        {
          title: "RAINBOWSIX SIEGE",
          sale: 80,
          price: 7990,
          genre: "Шутер",
          description:
            "Экшн-шутер в жанре зомби-апокалипсиса и с элементами строительства базы. Начните свой путь!",
        },
        {
          title: "RAINBOWSIX SIEGE",
          sale: 80,
          price: 7990,
          genre: "Шутер",
          description:
            "Экшн-шутер в жанре зомби-апокалипсиса и с элементами строительства базы. Начните свой путь!",
        },
        {
          title: "RAINBOWSIX SIEGE",
          sale: 80,
          price: 7990,
          genre: "Шутер",
          description:
            "Экшн-шутер в жанре зомби-апокалипсиса и с элементами строительства базы. Начните свой путь!",
        },
      ],
    };
  },
};
</script>