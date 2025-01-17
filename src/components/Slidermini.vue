<template>
  <div class="slider">
    <div class="slider__container" :style="{ transform: `translateX(-${currentIndex * 100}%)` }">
      <div v-for="(image, index) in images" :key="index" class="slider__item">
        <img :src="image" :alt="'Slide ' + (index + 1)" />
      </div>
    </div>

    <button class="slider__btn slider__btn--prev" @click="prevSlide">
      &#9664;
    </button>
    <button class="slider__btn slider__btn--next" @click="nextSlide">
      &#9654;
    </button>

    <div class="slider__indicators">
      <span v-for="(image, index) in images" :key="index"
        :class="['slider__indicator', { active: index === currentIndex }]" @click="goToSlide(index)"></span>
    </div>
  </div>
</template>

<script>
export default {
  name: "Slider",
  props: {
    images: {
      type: Array,
      required: true,
    },
  },
  data() {
    return {
      currentIndex: 0,
    };
  },
  methods: {
    nextSlide() {
      if (this.currentIndex < this.images.length - 1) {
        this.currentIndex++;
      } else {
        this.currentIndex = 0;
      }
    },
    prevSlide() {
      if (this.currentIndex > 0) {
        this.currentIndex--;
      } else {
        this.currentIndex = this.images.length - 1;
      }
    },
    goToSlide(index) {
      this.currentIndex = index;
    },
  },
};
</script>

<style scoped>
.slider {
  position: relative;
  width: 580px;
  height: 350px;
  overflow: hidden;
  border-radius: 20px;

}

.slider::before {
  content: '';
  position: absolute;
  top: 0;
  right: 20px;
  width: 60px;
  height: 60px;
  border-radius: 50%;
  background: linear-gradient(-120deg, rgba(67, 97, 238, 1), rgba(67, 97, 238, 0));
}

.slider__container {
  display: flex;
  transition: transform 0.5s ease;
}

.slider__item {
  min-width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
}

.slider__item img {
  width: 100%;
  height: 100%;
}

.slider__btn {
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  background-color: rgba(0, 0, 0, 0.5);
  color: #fff;
  border: none;
  padding: 10px 15px;
  cursor: pointer;
  font-size: 18px;
  border-radius: 50%;
}

.slider__btn--prev {
  left: 5px;
}

.slider__btn--next {
  right: 5px;
}

.slider__indicators {
  position: absolute;
  bottom: 10px;
  left: 50%;
  transform: translateX(-50%);
  display: flex;
  gap: 5px;
}

.slider__indicator {
  width: 10px;
  height: 10px;
  background-color: #ccc;
  border-radius: 50%;
  cursor: pointer;
}

.slider__indicator.active {
  background-color: #333;
}
</style>
