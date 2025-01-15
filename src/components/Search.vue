<script>
export default {

}
</script>
<template>
  <div class="realestate__search _text_1">
    <div class="realestate__switch "><span class="switch__item">For Sale</span><span class="switch__item">For
        Rent</span></div>
    <div class="search__item">
      <label for="city">New York, San Francisco, etc</label>
      <input type="text" placeholder="" id="city">
    </div>
    <div class="search__item">
      <label for="">Select Property Type</label>
      <select v-model="selected" class="property" id="property">
        <option value="a">A</option>
        <option value="b">B</option>
        <option value="c">C</option>
      </select>
    </div>
    <div class="search__item">
      <select v-model="selected" class="property" id="property__rooms">
        <option value="a">1</option>
        <option value="b">2</option>
        <option value="c">3</option>
      </select>
    </div>
  </div>
</template>



<style>
.realestate__search {
  width: 420px;
  height: 100px;
  display: flex;
  flex-direction: column;
  align-items: start;
  justify-content: center;
  gap: 30px;
  padding: 60px 40px;
  border-radius: 30px;
  background-color: #fff;
}

.realestate__switch {
  width: 100%;
  height: 80px;
  display: flex;
  align-items: center;
  justify-content: space-around;
  border-bottom: 2px solid #aaaaaa;
}

.switch__item {
  width: 100%;
  text-align: center;
  padding: 27px 43px;
}

.switch__item:hover {
  border-bottom: 2px solid var(--primary-colour);
  transition: all .6s ease-in-out;
}
</style>