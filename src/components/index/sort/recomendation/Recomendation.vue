<template>
  <div class="recomendation">
    <div class="recomendation__wrapper">
      <div class="recomendation__lists" v-for="item in items" :key="item">
        {{ item.title }}
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      items: [
        { title: "MMORPG" },
        { title: "Шутер" },
        { title: "Казуальные" },
        { title: "MMORPG" },
        { title: "Шутер" },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "./Recomendation.scss";
</style>