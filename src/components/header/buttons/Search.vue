<template>
  <transition name="slide-fade">
    <div v-if="show" class="search__input-main">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        width="22"
        height="22"
        fill="#454549"
        class="bi bi-search"
        viewBox="0 0 16 16"
      >
        <path
          d="M11.742 10.344a6.5 6.5 0 1 0-1.397 1.398h-.001c.03.04.062.078.098.115l3.85 3.85a1 1 0 0 0 1.415-1.414l-3.85-3.85a1.007 1.007 0 0 0-.115-.1zM12 6.5a5.5 5.5 0 1 1-11 0 5.5 5.5 0 0 1 11 0z"
        />
      </svg>
      <input class="search__input" type="text" placeholder="Поиск по сайту" />
      <div @click="modal" v-if="show" class="search__close"></div>
    </div>
  </transition>
  <button @click="modal" v-if="!show">
    <svg
      xmlns="http://www.w3.org/2000/svg"
      width="24"
      height="24"
      fill="white"
      class="bi bi-search"
      viewBox="0 0 16 16"
    >
      <path
        d="M11.742 10.344a6.5 6.5 0 1 0-1.397 1.398h-.001c.03.04.062.078.098.115l3.85 3.85a1 1 0 0 0 1.415-1.414l-3.85-3.85a1.007 1.007 0 0 0-.115-.1zM12 6.5a5.5 5.5 0 1 1-11 0 5.5 5.5 0 0 1 11 0z"
      />
    </svg>
  </button>
</template>

<script>
export default {
  data: function () {
    return {
      show: false,
    };
  },
  methods: {
    modal: function () {
      this.show = !this.show;
    },
  },
};
</script>

<style lang="scss">
.slide-fade-enter-active {
  transition: all 0.2s ease-out;
}

.slide-fade-leave-active {
  transition: all 0.2s;
}

.slide-fade-enter-from,
.slide-fade-leave-to {
  transform: translateX(20px);
  opacity: 0;
}
.search__input-main {
  position: relative;
  & svg {
    left: -83px;
    top: 6px;
    position: absolute;
    z-index: 999;
  }
}
.search__input {
  color: #f5f5f7;
  font-size: 16px;
  line-height: 19px;
  outline: none;
  padding: 8px 35px 7px 54px;
  width: 100%;
  min-width: 374px;
  border: 1.4px solid hsla(0, 0%, 100%, 0.4);
  border-radius: 6px;
  background: rgba(238, 235, 240, 0.08) 14px 50%/20px auto no-repeat;
  transform: translateX(-100px);
  position: relative;
  z-index: 999;
}
.search__close {
  cursor: pointer;
  top: 17px;
  right: 40px;
  position: absolute;
  z-index: 999;
}
.search__close:before,
.search__close:after {
  content: "";
  cursor: pointer;
  position: absolute;
  width: 24px;
  height: 3px;
  background: #454549;
  border-radius: 8px;
}
.search__close:before {
  transform: rotate(45deg);
}
.search__close:after {
  transform: rotate(-45deg);
}
button {
  position: relative;
  display: inline-block;
  vertical-align: middle;
  line-height: 21px;
  white-space: nowrap;
  cursor: pointer;
  background: none;
  border: none;
  outline: none;
  transition: 0.2s;
  padding: 6px;
  border-radius: 8px;
  display: flex;
  margin-right: 8px;
  &:hover {
    background-color: rgba(50, 50, 54, 0.9);
  }
}
@media (max-width: 1143px) {
  .search__input {
    min-width: 300px;
  }
}
@media (max-width: 1067px) {
  .search__input {
    min-width: 180px;
  }
}
@media (max-width: 967px) {
  .search__input {
    min-width: 100px;
  }
}
@media (max-width: 856px) {
  .search__input {
    min-width: 80px;
  }
}
@media (max-width: 768px) {
  .slide-fade-enter-from,
  .slide-fade-leave-to {
    transform: translateX(-20px);
    opacity: 0;
  }
  .search__input-main {
    position: absolute;
    width: 72%;
    right: 105px;
  }
  .search__input {
    background: #242429;
    min-width: 80px;
  }
}
@media (max-width: 736px) {
  .search__input-main {
    width: 70%;
  }
}
@media (max-width: 700px) {
  .search__input-main {
    width: 69%;
  }
}
@media (max-width: 662px) {
  .search__input-main {
    width: 66%;
  }
}
@media (max-width: 606px) {
  .search__input-main {
    width: 63%;
  }
}
@media (max-width: 550px) {
  .search__input-main {
    width: 46%;
  }
}
@media (max-width: 425px) {
  .search__input-main {
    right: 22px;
    width: 68%;
  }
  .search__input {
    width: 74%;
  }
  .search__close {
    right: 117px;
  }
}
</style>
