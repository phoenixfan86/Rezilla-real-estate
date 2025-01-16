<script>
import Slidermini from "./Slidermini.vue";
import Search from "./Search.vue";
export default {
  components: { Search, Slidermini },
  data() {
    return {
      imageList: [
        "./src/assets/img/gallery/1.png",
        "./src/assets/img/gallery/2.png",
        "./src/assets/img/gallery/3.png"
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

<style>
.block__wrapper {
  width: 100%;
  display: flex;
  align-items: center;
  justify-self: start;
  padding: 89px 140px;
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
