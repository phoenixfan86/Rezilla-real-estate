<script>
import Buttonlarge from "./Buttons/Buttonlarge.vue";

export default {
  components: { Buttonlarge },
  data() {
    return {
      selectedProperty: null,
      selectedRoom: null,
      propertyTypes: [
        { value: 'house', text: 'House' },
        { value: 'apartment', text: 'Apartment' },
        { value: 'cottage', text: 'Cottage' }
      ],
      roomsQuantity: [
        { value: '1', text: 'One room' },
        { value: '2', text: 'Two rooms' },
        { value: '3', text: 'Three rooms' },
        { value: '4', text: 'Four rooms' },
        { value: '5', text: 'Five rooms' }
      ]
    }
  }
}
</script>
<template>
  <div class="realestate__search _text_1">
    <div class="realestate__switch "><span class="switch__item">For Sale</span><span class="switch__item">For
        Rent</span></div>
    <div class="search__item">
      <label for="city">Select City</label>
      <input type="text" placeholder="" id="city" class="_item">
    </div>
    <div class="search__item">
      <label for="">Select Property Type</label>
      <select v-model="selectedProperty" class="property _item">
        <option v-for="property in propertyTypes" :key="property.value" :value="property.value"> {{ property.text }}
        </option>
      </select>
    </div>
    <div class="search__item">
      <label for="">Select Rooms</label>
      <select v-model="selectedRoom" class="property _item">
        <option v-for="quantity in roomsQuantity" :key="quantity.value" :value="quantity.value"> {{ quantity.text }}
        </option>
      </select>
    </div>
    <div class="search__block">
      <div class="search__wrapper">
        <div class="advanced__search">
          <a href="">
            <img src="/src/assets/img/ico/setting_ico.png" alt="">
            <span class="_smallp">Advance Search</span>
          </a>
        </div>
        <Buttonlarge label="Search">
          <template #icon>
            <img src="/src/assets/img/ico/search_ico.png" alt="icon" />
          </template>
        </Buttonlarge>
      </div>
    </div>
  </div>
</template>

<style scoped>
.realestate__search {
  width: 420px;
  height: auto;
  display: flex;
  flex-direction: column;
  align-items: start;
  justify-content: center;
  gap: 20px;
  padding: 50px 40px;
  border-radius: 30px;
  background-color: #fff;
  filter: drop-shadow(0 0 50px var(--text-1));
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
  color: var(--primary-colour);
  font-weight: medium;
  transition: all .4s ease-in-out;
}

.search__item {
  width: 100%;
  border-bottom: 1px solid #d4d4d4;
}

._item {
  width: 100%;
  height: 60px;
  border: 0;
  padding: 15px 10px 2px 10px;
  font-size: 18px;
  color: var(--text-1);
  outline: none;
}

.search__block {
  width: 100%;
}

.search__wrapper {
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  gap: 40px;
}

.advanced__search a {
  width: 135px;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 10px;
  color: var(--primary-colour);
}
</style>