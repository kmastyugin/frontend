<template>
  <div class="popular__categories">
    <h2>Популярные категории</h2>
    <div class="popular__categories-items">
      <RouterLink to="/" v-for="item in items" :key="item">
        <span>
          <svg xmlns="http://www.w3.org/2000/svg" x="0px" y="0px" width="24" height="24" viewBox="0 0 172 172"
            style="fill: #26e07f">
            <g fill="none" fill-rule="nonzero" stroke="none" stroke-width="1" stroke-linecap="butt"
              stroke-linejoin="miter" stroke-miterlimit="10" stroke-dasharray="" stroke-dashoffset="0"
              font-family="none" font-weight="none" font-size="none" text-anchor="none" style="mix-blend-mode: normal">
              <path d="M0,172v-172h172v172z" fill="none"></path>
              <g fill="#1fb141">
                <path
                  d="M21.5,21.5v129h64.5v-32.25v-64.5v-32.25zM86,53.75c0,17.7805 14.4695,32.25 32.25,32.25c17.7805,0 32.25,-14.4695 32.25,-32.25c0,-17.7805 -14.4695,-32.25 -32.25,-32.25c-17.7805,0 -32.25,14.4695 -32.25,32.25zM118.25,86c-17.7805,0 -32.25,14.4695 -32.25,32.25c0,17.7805 14.4695,32.25 32.25,32.25c17.7805,0 32.25,-14.4695 32.25,-32.25c0,-17.7805 -14.4695,-32.25 -32.25,-32.25z">
                </path>
              </g>
            </g>
          </svg>
        </span>
        <div>{{ item.title }}</div>
      </RouterLink>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [
        { img: "", title: "Бесплатные игры" },
        { img: "", title: "Бесплатные игры" },
        { img: "", title: "Бесплатные игры" },
        { img: "", title: "Бесплатные игры" },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "./Popular.scss";
</style>