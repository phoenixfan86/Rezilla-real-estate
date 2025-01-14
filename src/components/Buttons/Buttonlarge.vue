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
  <div class="button">
    {{ label }}
  </div>
</template>

<style></style>