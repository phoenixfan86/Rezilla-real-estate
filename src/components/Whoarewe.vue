<script>
export default {

}
</script>
<template>
  <div class="block__wrapper">
    <div class="inform">
      <div class="_label">who are we</div>
      <h2>Assisting individuals in locating the appropriate real estate.</h2>
      <p class="_text_1">Donec porttitor euismod dignissim. Nullam a lacinia ipsum, nec dignissim purus. Nulla convallis
        ipsum molestie
        nibh malesuada, ac malesuada leo volutpat.</p>
      <div class="sub__block">
        <img src="/public/img/ico/Vector-1.png" alt="">
        <div class="desc">
          <div class="_label">Donec porttitor euismod</div>
          <p class="_text_1">Nullam a lacinia ipsum, nec dignissim purus. Nulla</p>
        </div>
      </div>
      <div class="sub__block">
        <img src="/public/img/ico/Vector.png" alt="">
        <div class="desc">
          <div class="_label">Donec porttitor euismod</div>
          <p class="_text_1">Nullam a lacinia ipsum, nec dignissim purus. Nulla</p>
        </div>
      </div>
    </div>
    <div class="img_wrapper">
      <div class="img__item">
        <img src="/img/gallery/3.png" alt="">
      </div>
      <div class="img__item_1">
        <img src="/public/img/gallery/2.png" alt="">
        <img src="/public/img/gallery/4.png" alt="">
      </div>
    </div>
  </div>
</template>
<style scoped>
.block__wrapper {
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 30px;
  margin-top: 180px;
}

.inform {
  width: 500px;
  display: flex;
  flex-direction: column;
  align-items: start;
  justify-content: center;
  gap: 30px;
}

.sub__block {
  width: 400px;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 20px;
  padding: 20px;
}

.sub__block img {
  width: 40px;
  height: 40px;
}

.img_wrapper {
  width: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 5px;
}

.img__item {
  width: 280px;
  height: 500px;
}

.img__item img {
  width: 280px;
  height: 500px;
}

.img__item_1 {
  position: relative;
  width: 280px;
  height: 550px;
}

.img__item_1:nth-child(1) {
  width: 277px;
  height: 280px;
}

.img__item_1:nth-child(2):after {
  content: '';
  position: absolute;
  bottom: -30px;
  left: 30%;
  width: 60px;
  height: 60px;
  border-radius: 50%;
  background: linear-gradient(-120deg, rgba(67, 97, 238, 1), rgba(67, 97, 238, 0));
}
</style>