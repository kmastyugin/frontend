<template>
  <div class="filter__container">
    <div class="filter__item">
      <div class="filter__item-title">Тип</div>
      <div v-for="item in items" :key="item">
        <div class="filter__item-checkbox">
          <label>
            <input class="filter__item-input" type="checkbox" />
            <span class="filter__item-input-checkbox"></span>
            <span>{{ item.input }}</span>
          </label>
        </div>
      </div>
    </div>

    <div class="filter__item">
      <div class="filter__item-title">Особенность</div>
      <div v-for="item in items" :key="item">
        <div class="filter__item-checkbox">
          <label>
            <input class="filter__item-input" type="checkbox" />
            <span class="filter__item-input-checkbox"></span>
            <span>{{ item.input }}</span>
          </label>
        </div>
      </div>
    </div>

    <div class="filter__item">
      <div class="filter__item-title">Жанр</div>
      <div v-for="item in items" :key="item">
        <div class="filter__item-checkbox">
          <label>
            <input class="filter__item-input" type="checkbox" />
            <span class="filter__item-input-checkbox"></span>
            <span>{{ item.input }}</span>
          </label>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          input: "Мини игры",
        },
        {
          input: "Новинки",
        },
        {
          input: "Новинки",
        },
        {
          input: "Популярные",
        },
        {
          input: "Мини игры",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "./Checkbox.scss";
</style>
