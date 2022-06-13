<template>
  <!-- <Slider /> -->
  <section class="container">
    <div class="container__wrapper">
      <Selection />
      <div class="container_right">
        <Popular />
        <div class="recommendations">
          <div class="recommendations__wrapper">
            <div class="recommendations__title">
              <h2>Рекомендуемое</h2>
              <RouterLink to="/">Перейти в каталог</RouterLink>
            </div>
          </div>
        </div>
        <Recomendation />
        <List />
        <div class="recommendations">
          <div class="recommendations__title">
            <h2>Новинки</h2>
            <RouterLink to="/">Перейти в каталог</RouterLink>
          </div>
          <List />
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import Slider from "@/components/slider/Slider";
import Selection from "@/components/index/sort/selection/Selection";
import List from "@/components/global/goods/list/List";
import Recomendation from "@/components/index/sort/recomendation/Recomendation";
import Popular from "@/components/index/sort/popular/Popular";

export default {
  components: {
    Slider,
    Selection,
    List,
    Recomendation,
    Popular,
  },
};
</script>
<style lang="scss" scoped>
.container {
  padding-left: 30px;
  padding-right: 30px;
  width: 1380px;
  margin: 0 auto;
}

.container__wrapper {
  display: flex;
  align-items: stretch;
  padding: 26px 0;
}

.container_right {
  width: 73%;
  margin: 0 auto;
}

@media (max-width: 1522px) {
  .container {
    width: 1080px;
  }
}

@media (max-width: 1122px) {
  .container {
    width: 800px;
  }

  .container_right {
    width: 500px;
  }
}

@media (max-width: 980px) {
  .container {
    width: 90%;
  }
}

@media (max-width: 585px) {
  .container_right {
    width: 97%;
  }
}

@media (max-width: 455px) {
  .container {
    width: 83%;
    padding: 0;
  }

  .container_right {
    width: 100%;
  }
}
</style>