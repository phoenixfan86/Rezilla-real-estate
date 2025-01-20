<script>
export default {

}
</script>

<template>
  <div class="user__login">
    <div class="user__login__wrapper">
      <a href="" class="login__block _text_2">
        <div class="login__img"><img src="/public/img/ico/user_ico.png" alt="userico"></div>
        Login/Register
      </a>
    </div>
  </div>
</template>

<style>
.user__login {
  width: 150px;
  display: flex;
  align-items: center;
  justify-content: center;
}

.user__login__wrapper {
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;

  gap: 10px;
}

.login__img {
  width: 20px;
  height: 20px;
}

.login__block {
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 8px;
}

.user__login__wrapper a {
  color: var(--text-2);
}
</style>
