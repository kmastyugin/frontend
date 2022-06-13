<template>
  <div class="pagination">
    <ul class="pagination__numbers">
      <li>
        <a class="pagination__arrow arrow-right" href="/">
          <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor"
            class="bi bi-caret-right-fill" viewBox="0 0 16 16">
            <path
              d="m12.14 8.753-5.482 4.796c-.646.566-1.658.106-1.658-.753V3.204a1 1 0 0 1 1.659-.753l5.48 4.796a1 1 0 0 1 0 1.506z" />
          </svg>
        </a>
      </li>
      <li class="pagination__action-link"><a href="/">1</a></li>
      <li><a href="/">2</a></li>
      <li><a href="/">3</a></li>
      <li>...</li>
      <li><a href="/">4</a></li>
      <li><a href="/">5</a></li>
      <li>
        <a class="pagination__arrow" href="/">
          <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor"
            class="bi bi-caret-right-fill" viewBox="0 0 16 16">
            <path
              d="m12.14 8.753-5.482 4.796c-.646.566-1.658.106-1.658-.753V3.204a1 1 0 0 1 1.659-.753l5.48 4.796a1 1 0 0 1 0 1.506z" />
          </svg>
        </a>
      </li>
    </ul>
    <div class="pagination__results">
      <div class="pagination__show">
        <span>Показано 1 — 48 из</span>
        <span>1234</span>
      </div>
      <div class="pagination__show">
        <div class="pagination__limitText">Показывать по:</div>
        <ul class="pagination__numbers">
          <li class="pagination__action-link"><a href="/">11</a></li>
          <li><a href="/">22</a></li>
          <li><a href="/">23</a></li>
        </ul>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@import "./Pagination.scss";
</style>
