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
            <div class="title">Об игре</div>
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
          <div class="title">Вам может понравиться</div>
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
            <div class="title">Информация об игре</div>
            <ul class="game__item-lists-info">
              <li>
                <div>Жанр</div>
                <div>Экшен, Шутер</div>
              </li>
              <li>
                <div>Издатель</div>
                <div>Экшен, Шутер</div>
              </li>
              <li>
                <div>Техническая поддержка</div>
                <div>Экшен, Шутер</div>
              </li>
              <li>
                <div>Дата выхода</div>
                <div>Экшен, Шутер</div>
              </li>
              <li>
                <div>Размер дистрибутива</div>
                <div>Экшен, Шутер</div>
              </li>
              <li>
                <div>Теги</div>
                <div>
                  <ul>
                    <li>
                      <router-link to="/">Экшен</router-link>
                    </li>
                    <li>
                      <router-link to="/">Шутер</router-link>
                    </li>
                  </ul>
                </div>
              </li>
            </ul>
          </div>
        </div>

        <div class="game__item-container-right-info">
          <div class="game__item-container-box">
            <div class="title">Атрибуты</div>
            <ul class="game__item-lists-info">
              <li>
                <span>
                  <div class="icon voz-0"></div> Возрастное ограничение
                </span>
              </li>
              <li>
                <span>
                  <div class="icon client"></div> Клиентская-игра
                </span>
              </li>
              <li>
                <span>
                  <div class="icon online"></div> Онлайн-игра
                </span>
              </li>
            </ul>
          </div>
        </div>
        <div class="game__item-container-right-info">
          <div class="game__item-container-box">
            <div class="title">Системные требования</div>
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
// import SliderInPage from "@/components/slider/SliderInPage";

export default {
  // components: {
  //   SliderInPage,
  // },
  data() {
    return {
      ImgItem: require("@/assets/imgs/game-page/Battlegrounds.jpg"),
    };
  },
};
</script>

<style lang="scss">
@import "./GoodsPage.scss";
</style>