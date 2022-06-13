<template>
  <a class="button__up" href="/">
    <span>Наверх</span>
  </a>
</template>

<style lang="scss" scoped>
.button__up {
  display: block;
  position: fixed;
  z-index: 900;
  bottom: 72px;
  left: 20px;
  padding: 8px 20px;
  text-align: center;
  text-decoration: none;
  border-radius: 4px;
  box-shadow: 0 2px 6px rgb(0 0 0 / 11%);
  opacity: 1;
  transition: opacity 0.6s, z-index 0.6s;
  cursor: pointer;
  background-color: #363636;
  & span {
    font-size: 14px;
    font-weight: 700;
    letter-spacing: 0.6px;
    color: #f5f5f7;
    opacity: 0.7;
    -webkit-transition: opacity 0.1s;
    transition: opacity 0.1s;
  }
  &:hover {
    & span {
      color: #ffffff;
    }
  }
}
@media (max-width: 820px) {
  .button__up {
    display: none;
  }
}
</style>