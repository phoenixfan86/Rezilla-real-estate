<script>
export default {
  name: 'Buttonlarge',
  props: {
    label: {
      type: String,
      required: true
    }
  }
}
</script>

<template>
  <a href="">
    <div class="button__large">
      <slot name="icon"></slot>
      {{ label }}
    </div>
  </a>
</template>

<style>
.button__large {
  width: 170px;
  height: 50px;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 10px;
  padding: 15px 20px;
  border-radius: 50px;
  background-color: var(--primary-colour);
  color: #fff;
}

.button__large:hover {
  filter: drop-shadow(0 0 30px var(--text-1));
  transform: scale(.98);
  transition: all .7s cubic-bezier(0.075, 0.82, 0.165, 1);
}
</style>