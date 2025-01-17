<script>
export default {
  data() {
    return {
      imagesList: [
        './img/Brands/image-1.png',
        './img/Brands/image-2.png',
        './img/Brands/image-3.png',
        './img/Brands/image-4.png',
        './img/Brands/image-5.png',
        './img/Brands/image-6.png'
      ]
    }

  }

}
</script>
<template>
  <div class="block__wrapper">
    <p>Trusted by 100+ Companies across the globe! </p>
    <div class="logotipe">
      <div class="item" v-for="(logo, index) in imagesList" :key="index">
        <img :src="logo" :alt="'Brand' + (index + 1)">
      </div>
    </div>
  </div>
</template>
<style scoped>
.block__wrapper {
  position: relative;
  width: 100%;
  height: 200px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  gap: 50px;
  margin-top: 50px;
  padding: 40px 100px;
  color: var(--text-1);
}


.block__wrapper:after {
  content: '';
  position: absolute;
  top: -15px;
  left: 150px;
  width: 100px;
  height: 100px;
  background: linear-gradient(150deg, rgba(67, 97, 238, .8), rgba(67, 97, 238, 0));
  border-radius: 50%;
}

.logotipe {
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.item {
  filter: grayscale(1);
}

.item:hover {
  filter: grayscale(0);
  transition: all .7s cubic-bezier(0.175, 0.885, 0.32, 1.275);
}
</style>