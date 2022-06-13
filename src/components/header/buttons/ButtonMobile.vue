<template>
  <button class="registration">
    <slot></slot>
  </button>
</template>
<style lang="scss" scoped>
.registration {
  padding: 8px 48px;
  box-sizing: border-box;
  margin-right: 11px;
  background-color: #e2e3e7;
  border-radius: 6px;
  border: none;
}
@media (max-width: 356px) {
  .registration {
    margin-right: 0;
    padding: 8px 32px;
  }
}
</style>