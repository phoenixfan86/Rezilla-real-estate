<script>
export default {
  name: 'ListingsNewTab',
  props: {
    label: {
      type: String,
      required: true
    }
  }
}
</script>

<template>
  <div class="listings__tab">
    <slot name="icon"></slot>
    {{ label }}
  </div>
</template>

<style scoped>
.listings__tab {
  width: 320px;
  height: 100px;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 10px;
  padding: 20px 38px;
  border-radius: 50px;
  background-color: #fff;
  filter: drop-shadow(0 0 10px var(--text-1));
  font-size: 18px;
  font-weight: 600;
  margin-top: 20px;
}
</style>