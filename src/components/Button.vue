<script>
export default {
  props: {
    label: {
      type: String,
      required: true
    }
  }
}
</script>
<template>
  <div class="button">
    {{ label }}
  </div>
</template>

<style>
.button {
  width: 100%;
  height: 100%;
  padding: 13px 16px;
  border-radius: 30px;
}

.button:hover {
  background-color: var(--button-hover);
  transition: all .7s ease;
}
</style>