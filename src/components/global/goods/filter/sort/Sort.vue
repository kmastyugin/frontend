<template>
  <div class="filter__sort">
    <span>Сначала:</span>

    <div :class="[{ visible: visibleMenu }]" class="select" @click.stop="switchMenu">
      {{ selectedOption.name }}
    </div>

    <div v-if="visibleMenu" ref="menu" class="filter__sort-value">
      <span class="selectOption active" @click.stop="switchMenu"> {{ selectedOption.name }} </span>
      <span v-for="option in sortedOptions" :key="option.value" @click="selectOption(option)">{{ option.name }}</span>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      selectedOption: { name: "рекомендуемые", value: 1 },
      visibleMenu: false,
      options: [
        { name: "рекомендуемые", value: 1 },
        { name: "по дате выхода", value: 2 },
        { name: "по дате выхода", value: 3 },
        { name: "по дате выхода", value: 4 },
      ],
    };
  },

  computed: {
    sortedOptions() {
      return this.options.filter((option) => option.value !== this.selectedOption.value);
    }
  },
  watch: {
    visibleMenu() {
      if (this.visibleMenu) {
        document.removeEventListener('click', this.clickPastMenu);
        document.addEventListener('click', this.clickPastMenu);
      } else {
        document.removeEventListener('click', this.clickPastMenu);
      }
    }
  },
  methods: {
    selectOption(option) {
      this.selectedOption = option;
    },

    // Если клик мимо меню - удалить слушатель и 
    clickPastMenu(e) {
      if (this.$refs.menu !== e.target) {
        document.removeEventListener('click', this.clickPastMenu);
        this.visibleMenu = false;
      }
    },

    switchMenu() {
      // Переключить видимость меню
      this.visibleMenu = !this.visibleMenu;
    }
  },
};
</script>

<style lang="scss" scoped>
@import "./Sort.scss";
</style>
