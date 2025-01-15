<script>
import Search from "./Search.vue";
export default {
  components: { Search }
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
      <div class="gallery__preview"></div>
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