<script>
import Slidermini from "./Slidermini.vue";
import Search from "./Search.vue";
export default {
  components: { Search, Slidermini },
  data() {
    return {
      imageList: [
        "./img/gallery/1.png",
        "./img/gallery/2.png",
        "./img/gallery/3.png"
      ],
    }
  }
}
</script>
<template>
  <div class="block__wrapper">
    <div class="description__block">
      <span class="_label">real estate</span>
      <h1>Find a perfect home you love..!</h1>
      <p class="_text_1">Etiam eget elementum elit. Aenean dignissim dapibus vestibulum. Integer a dolor eu sapien
        sodales vulputate ac
        in
        purus.</p>
      <div class="gallery__preview">
        <Slidermini :images="imageList" />
      </div>
    </div>
    <Search />
  </div>
</template>

<style scoped>
.block__wrapper {
  position: relative;
  width: 100%;
  height: 900px;
  display: flex;
  align-items: center;
  justify-self: start;
  gap: 80px;
  padding: 40px 100px;
  overflow: hidden;
  z-index: 1;
}

.block__wrapper::before {
  position: absolute;
  top: -50%;
  left: 50%;
  transform: translateX(-50%);
  content: '';
  width: 100%;
  height: 1200px;
  border-radius: 50%;
  background: linear-gradient(0deg, rgba(67, 97, 238, .5), rgba(76, 201, 240, 0));
  z-index: -1;
}

.description__block {
  width: 580px;
  display: flex;
  flex-direction: column;
  align-items: start;
  justify-content: center;
  gap: 15px;
}
</style>
