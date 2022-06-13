<template>
  <div class="navigation__main">
    <ul class="navigation">
      <li>
        <RouterLink to="/goods">Игры</RouterLink>
      </li>
      <li>
        <RouterLink to="/goods">Библиотека</RouterLink>
      </li>
      <li>
        <RouterLink to="/goods">Акции</RouterLink>
      </li>
    </ul>
    <Search />
  </div>
</template>

<script>
import Search from "@/components/header/buttons/Search";
export default {
  components: { Search },
};
</script>

<style lang="scss">
@import "./Navigation.scss";
</style>
