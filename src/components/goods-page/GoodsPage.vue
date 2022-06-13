<template>
  <section class="game__item">
    <div class="game__item-inner">
      <p>Pubg (PlayerUnknown's Battlegrounds)</p>
      <a href="/">Купить </a>
    </div>
    <div class="game__item-container">
      <div class="game__item-container-left">
        <div class="game__item-container-left-info">
          <div class="game__item-container-box">
            <h2>Об игре</h2>
            <p>
              Warface — динамичный экшен в жанре MMOFPS с миллионами поклонников
              по всему миру. В игре вас ждут отличная графика, увлекательные
              PvP-бои и PvE-миссии, где вы можете испытать себя, играя 5
              различными классами, и у каждого из них своя тактика ведения боя.
              В PvE вам предстоит выполнять миссии в самых отдаленных уголках
              планеты, а в PvP играть в тактических режимах и динамичных боях на
              выживание.
            </p>
          </div>
        </div>
        <div class="game__item-container-left-info">
          <div class="game__item-container-box">
            <img class="game__item-previev"
              src="https://store.my.games/pre_310x186_resize/hotbox/showcase/game/picture/76178575-669c-4d8a-8d65-374a58d96feb.jpeg?quality=85&format=webp"
              alt="" />
            <p>
              Warface — динамичный экшен в жанре MMOFPS с миллионами поклонников
              по всему миру. В игре вас ждут отличная графика, увлекательные
              PvP-бои и PvE-миссии, где вы можете испытать себя, играя 5
              различными классами, и у каждого из них своя тактика ведения боя.
              В PvE вам предстоит выполнять миссии в самых отдаленных уголках
              планеты, а в PvP играть в тактических режимах и динамичных боях на
              выживание.
            </p>
          </div>
        </div>
        <div class="slider__container">
          <h2>Вам может понравиться</h2>
          <!-- <SliderInPage /> -->
        </div>
      </div>
      <div class="game__item-container-right">
        <div class="game__item-container-right-info">
          <img
            src="https://store.my.games/pre_310x186_resize/hotbox/showcase/gamelocale/picture/c4b0062f-8742-45c2-8320-73afec862399.jpg?quality=85&format=webp"
            alt="game" />
          <p>
            Вам предстоит вести сражения в различных уголках земного шара,
            начиная с городов и заканчивая самыми опасными местами на планете.
            Инновационный дизайн проекта сочетает простое управление и
            уникальный игровой процесс, позволяющий с головой окунуться в
            суровый мир будущего.
          </p>
        </div>
        <div class="game__item-container-right-info">
          <div class="game__item-container-box">
            <h2>Информация об игре</h2>
            <ul class="game__item-lists-info">
              <li>
                <p>Жанр</p>
                <p>Экшен, Шутер</p>
              </li>
              <li>
                <p>Издатель</p>
                <p>Экшен, Шутер</p>
              </li>
              <li>
                <p>Техническая поддержка</p>
                <p>Экшен, Шутер</p>
              </li>
              <li>
                <p>Дата выхода</p>
                <p>Экшен, Шутер</p>
              </li>
              <li>
                <p>Размер дистрибутива</p>
                <p>Экшен, Шутер</p>
              </li>
              <li>
                <p>Теги</p>
                <p>Экшен, Шутер</p>
              </li>
            </ul>
          </div>
        </div>
        <div class="game__item-container-right-info">
          <div class="game__item-container-box">
            <h2>Атрибуты</h2>
            <ul class="game__item-lists-info">
              <li>
                <p>Жанр</p>
                <p>Возрастное ограничение</p>
              </li>
              <li>
                <p>Издатель</p>
                <p>Клиентская</p>
              </li>
              <li>
                <p>Техническая</p>
                <p>Поддерживает запись видео</p>
              </li>
              <li>
                <p>Дата</p>
                <p>Поддерживает снятие скриншотов</p>
              </li>
            </ul>
          </div>
        </div>
        <div class="game__item-container-right-info">
          <div class="game__item-container-box">
            <h2>Системные требования</h2>
            <h4>Минимальные</h4>
            <ul class="game__item-list-system">
              <li>ОС: Windows XP</li>
              <li>Процессор: Intel Core 2 Duo</li>
              <li>Память: 2 ГБ</li>
              <li>Место на диске: 500 М</li>
              <li>Видеокарта: с 128 MB памяти</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import SliderInPage from "@/components/slider/SliderInPage";

export default {
  components: {
    SliderInPage,
  },
  data() {
    return {
      ImgItem: require("@/assets/imgs/game-page/Battlegrounds.jpg"),
    };
  },
};
</script>

<style lang="scss" scoped>
@import "./GoodsPage.scss";
</style>