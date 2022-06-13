<template>
  <RouterLink class="breadcrumbs__link" :to="link">
    <slot></slot>
  </RouterLink>
</template>

<script>
export default {
  props: {
    link: {
      type: String,
      default: "/",
      required: true,
    },
  },
};
</script>

<style lang="scss" scoped>
.breadcrumbs__link {
  padding: 8px 12px;
  font-size: 12px;
  line-height: 14px;
  text-decoration: none;
  color: #8f8f8f;
  text-shadow: 0 0 4px rgb(0 0 0 / 44%);
}
@media (max-width: 455px) {
  .breadcrumbs__link {
    padding: 0;
    padding-right: 10px;
  }
}
</style>