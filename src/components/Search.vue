<script>
export default {
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
  </div>
</template>



<style>
.realestate__search {
  width: 420px;
  height: auto;
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
</style>