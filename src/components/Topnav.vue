<script>
import Button from "./Buttons/Button.vue";
import Buttonlarge from "./Buttons/Buttonlarge.vue";
import Sitelogo from "./Sitelogo.vue";
import Userlogin from "./Userlogin.vue";

export default {
  components: { Button, Sitelogo, Userlogin }
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
    <Userlogin />
    <>
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
  width: 100%;
  height: 37px;
  display: flex;
  align-items: center;
  justify-content: center;
}
</style>