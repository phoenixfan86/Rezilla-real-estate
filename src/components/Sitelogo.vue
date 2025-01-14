<script>
export default {

}
</script>

<template>
  <div class="logo">
    <div class="logo__wrapper">
      <div class="logo__img">
        <img src="/src/assets/img/ico/house_ico.png" alt="">
      </div>
      <a href="#">
        <h4 class="_text_2">Rezilla</h4>
      </a>
    </div>

  </div>
</template>

<style>
.logo {
  width: 125px;
  height: 50px;
  display: flex;
}

.logo__wrapper {
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: space-between;
  font-size: 20px;
}

.logo__img {
  width: 50px;
  height: 50px;
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: var(--primary-colour);
  border-radius: 50%;
}
</style>