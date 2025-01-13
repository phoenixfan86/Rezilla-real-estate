<script>
import Button from "./Button.vue";
import Logo from "./Sitelogo.vue";

export default {
  components: { Button, Logo }
}
</script>
<template>
  <nav>
    <div class="top__menu">
      <ul class="top__menu__wrapper">
        <li><a href="#" class="menu__item"><Button class="_text_2" label="Home" /></a></li>
        <li><a href="#" class="menu__item"><Button class="_text_2" label="About" /></a></li>
        <li><a href="#" class="menu__item"><Button class="_text_2" label="Listings" /></a></li>
        <li><a href="#" class="menu__item"><Button class="_text_2" label="Services" /></a></li>
        <li><a href="#" class="menu__item"><Button class="_text_2" label="Blog" /></a></li>
      </ul>
    </div>
    <Logo />
    <div class="user__block">
      <div class="user__img"><a href=""><img src="/src/assets/img/ico/user_ico.png"
            alt=""><span>Login/Register</span></a></div>
    </div>
  </nav>
</template>

<style>
nav {
  width: 100%;
  height: 80px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 21px 100px;
}

.top__menu__wrapper {
  width: 100%;
  display: flex;
}
</style>