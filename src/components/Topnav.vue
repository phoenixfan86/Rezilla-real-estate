<script>
import Button from "./components/Button.vue";
import Sitelogo from "./components/Sitelogo.vue";
export default {
  components: { Button, Sitelogo },
}
</script>
<template>
  <nav>
    <div class="top__menu">
      <ul class="top__menu__wrapper">
        <li><a href="#" class="menu__item"><Button class="button _text_2" label="Home" /></a></li>
        <li><a href="#" class="menu__item"><Button class="button _text_2" label="Aboutus" /></a></li>
        <li><a href="#" class="menu__item"><Button class="button _text_2" label="Listings" /></a></li>
        <li><a href="#" class="menu__item"><Button class="button _text_2" label="Services" /></a></li>
        <li><a href="#" class="menu__item"><Button class="button _text_2" label="Blog" /></a></li>
      </ul>
    </div>
    <div class="logo">
    <Sitelogo />
    </div>
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

.menu__item {
  padding: 13px 16px;
}
</style>