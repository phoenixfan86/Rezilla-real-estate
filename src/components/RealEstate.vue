<script>
import Slidermini from "./Slidermini.vue";
import Search from "./Search.vue";
import ListingsNewTab from "./ListingsNewTab.vue";
export default {
  components: { Search, Slidermini, ListingsNewTab },
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
    <div class="content__wrapper">
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
    <ListingsNewTab label="200+ New 
Listings Everyday!">
      <template #icon>
        <img src="/public/img/gallery/house2.png" alt="icon" />
      </template>
    </ListingsNewTab>
  </div>
</template>

<style scoped>
.block__wrapper {
  width: 100%;
  height: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

.content__wrapper {
  position: relative;
  width: 100%;
  height: auto;
  display: flex;
  align-items: center;
  justify-self: start;
  gap: 80px;
  padding: 40px 100px;
  margin-bottom: 20px;

  z-index: 1;
}

.block__wrapper::before {
  position: absolute;
  top: -30%;
  left: 50%;
  transform: translateX(-50%);
  content: '';
  width: 105%;
  height: 1150px;
  border-radius: 50%;
  background: linear-gradient(0deg, rgba(67, 97, 238, .3), rgba(76, 201, 240, 0));
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

.gallery__preview {
  padding: 10px;
}
</style>
