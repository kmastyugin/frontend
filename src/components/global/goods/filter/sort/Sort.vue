<template>
  <div class="filter__sort">
    <div @click="show = !show">Сначала: {{ selectOption?.name }}</div>
    <div v-if="show" class="filter__sort-value">
      <span v-for="option in options" :key="option.value" @click="selectOptions(option)">{{ option.name }}</span>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      selectOption: null,
      show: false,
      options: [
        { name: "рекомендуемые", value: 1 },
        { name: "по дате выхода", value: 2 },
        { name: "по дате выхода", value: 3 },
        { name: "по дате выхода", value: 4 },
      ],
    };
  },
  methods: {
    selectOptions(option) {
      this.selectOption = option;
      this.show = false;
    },
    hideSelect() {
      this.show = false;
    },
  },
  mounted() {
    document.addEventListener("click", this.hideSelect.bind(this), true);
  },
  beforeDestroy() {
    document.removeEventListener("click", this.hideSelect);
  },
};
</script>

<style lang="scss" scoped>
@import "./Sort.scss";
</style>
