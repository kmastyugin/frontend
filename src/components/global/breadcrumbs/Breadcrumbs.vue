<template>
  <div class="breadcrumbs">
    <ul>
      <li>
        <BreadcrumbsItem link="/">STEAM GAME</BreadcrumbsItem>
      </li>
      <li>
        <BreadcrumbsItem link="/">Популярные игры</BreadcrumbsItem>
      </li>
    </ul>
  </div>
</template>
<script>
import BreadcrumbsItem from "@/components/global/breadcrumbs/BreadcrumbsItem";
export default {
  components: { BreadcrumbsItem },
};
</script>
<style lang="scss" scoped>
.breadcrumbs {
  padding: 20px 0;

  & ul {
    display: flex;
    padding: 12px 0 0 0;
    margin: 0;
    list-style: none;
  }
}

@media (max-width: 1100px) {
  .breadcrumbs {
    width: 100%;
    max-width: 472px;
    padding-right: 30px;
    margin: 0 auto;
  }
}

@media (max-width: 600px) {
  .breadcrumbs {
    width: 93%;
  }
}
</style>