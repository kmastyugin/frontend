<template>
  <header>
    <nav class="header__wrapper">
      <Burger />
      <Logo />
      <Navigation />
      <Authorization />
    </nav>
  </header>
</template>

<script>
import Navigation from "@/components/header/navigation/Navigation";
import Logo from "@/components/header/logo/Logo";
import Authorization from "@/components/header/buttons/Authorization";
import Burger from "@/components/header/burger/Burger";

export default {
  components: { Navigation, Logo, Authorization, Burger },
};
</script>
<style lang="scss">
@import "./Header.scss";
</style>
