<template>
  <div class="recommendations__items">
    <ul>
      <li v-for="item in items" :key="item">
        <Good :item="item" />
      </li>
    </ul>
    <ButtonShowMore />
  </div>
</template>

<script>
import ButtonShowMore from "@/components/index/buttons/ButtonShowMore";
import Good from "@/components/global/goods/Good";

export default {
  components: {
    ButtonShowMore,
    Good,
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

<style lang="scss">
@import "./List.scss";
</style>