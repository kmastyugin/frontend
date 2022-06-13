<template>
  <div class="show-more-button">Показать еще</div>
</template>
<style lang="scss" scoped>
.show-more-button {
  display: block;
  padding: 13px;
  font-size: 1rem;
  font-weight: 500;
  line-height: normal;
  text-align: center;
  width: 100%;
  margin: 0;
  border-radius: 6px;
  cursor: pointer;
  -webkit-transition: all 0.1s;
  transition: all 0.1s;
  outline: none;
  color: rgba(245, 245, 247, 0.7);
  background-color: #272728;
  box-sizing: border-box;

  &:hover {
    color: #f5f5f7;
  }
}

@media (max-width: 455px) {
  .show-more-button {
    width: 90%;
  }
}
</style>