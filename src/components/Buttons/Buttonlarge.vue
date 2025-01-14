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
  justify-self: start;
  gap: 10px;
  padding: 15px 20px;
  border-radius: 50px;
  background-color: var(--primary-colour);
  color: #fff;
}
</style>