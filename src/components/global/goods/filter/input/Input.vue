<template>
  <div class="filter__input">
    <div class="filter__input-wrapper">
      <div class="filter__input-search">
        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="#59595c" class="bi bi-search"
          viewBox="0 0 16 16">
          <path
            d="M11.742 10.344a6.5 6.5 0 1 0-1.397 1.398h-.001c.03.04.062.078.098.115l3.85 3.85a1 1 0 0 0 1.415-1.414l-3.85-3.85a1.007 1.007 0 0 0-.115-.1zM12 6.5a5.5 5.5 0 1 1-11 0 5.5 5.5 0 0 1 11 0z" />
        </svg>
        <input type="text" placeholder="Поиск по каталогу" />
      </div>
    </div>
    <FilterSort />
  </div>
</template>

<script>
import FilterSort from "@/components/global/goods/filter/sort/Sort";

export default {
  components: { FilterSort },
};
</script>

<style lang="scss" scoped>
@import "./Input.scss";
</style>