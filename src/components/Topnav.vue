<script>
export default {

}
</script>
<template>
  <nav>
    <div class="top__menu">
      <ul class="top__menu__wrapper">
        <li><a href="#" class="menu__item">Home</a></li>
        <li><a href="#" class="menu__item">About-me</a></li>
        <li><a href="#" class="menu__item">Listings</a></li>
        <li><a href="#" class="menu__item">Services</a></li>
        <li><a href="#" class="menu__item">Blog</a></li>
      </ul>
    </div>
    <div class="logo">
      <div class="logo__img">
        <a href="#">
          <img src="/src/assets/img/ico/house_ico.png" alt="">
          <h4>Rezilla</h4>
        </a>
      </div>
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