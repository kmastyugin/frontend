<template>
  <a class="user__icon" href="/">
    <svg
      xmlns="http://www.w3.org/2000/svg"
      width="24"
      height="24"
      fill="white"
      class="bi bi-person-circle"
      viewBox="0 0 16 16"
    >
      <path d="M11 6a3 3 0 1 1-6 0 3 3 0 0 1 6 0z" />
      <path
        fill-rule="evenodd"
        d="M0 8a8 8 0 1 1 16 0A8 8 0 0 1 0 8zm8-7a7 7 0 0 0-5.468 11.37C3.242 11.226 4.805 10 8 10s4.757 1.225 5.468 2.37A7 7 0 0 0 8 1z"
      />
    </svg>
    <span class="user__login">Войти</span>
  </a>
</template>
<script>
export default {};
</script>
<style lang="scss">
.user__icon {
  display: flex;
  align-items: center;
  text-decoration: none;
  transition: 0.2s;
  padding: 6px;
  border-radius: 8px;
  &:hover {
    background-color: rgba(50, 50, 54, 0.9);
  }
}
.user__login {
  display: inline-block;
  padding: 6px;
  font-size: 14px;
  font-weight: 500;
  color: #fff;
  text-decoration: none;
  opacity: 0.8;
  transition: opacity 0.1s;
  cursor: pointer;
}
@media (max-width: 490px) {
  .user__login {
    display: none;
  }
}
</style>
