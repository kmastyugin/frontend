<template>
  <section class="game__page">
    <Breadcrumbs />
    <GoodsPage />
  </section>
</template>

<script>
import GoodsPage from "@/components/goods-page/GoodsPage";
import Breadcrumbs from "@/components/global/breadcrumbs/Breadcrumbs";

export default {
  components: {
    GoodsPage,
    Breadcrumbs,
  },
};
</script>
<style lang="scss" scoped>
.game__page {
  width: 90vw;
  margin: 0 auto;
}
</style>