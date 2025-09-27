<script setup>
import Arrow from '@/assets/SVG (1).svg'

defineProps({
  txt: {
    type: String,
    required: true,
  },
})
</script>
<template>
  <button>
    {{ txt }}
  </button>
</template>
<style scoped>
button {
  border: none;
  display: flex;
  align-items: center;
  gap: 10px;
  width: fit-content;
  background-color: #fff;
  border: 2px solid #000;
  padding: 13px 23px;
  color: #000;
  font-weight: 300;
  border-radius: 96px;
  cursor: pointer;
  font-weight: 400;
  line-height: 19.5px;
  letter-spacing: 0.13px;
}
</style>
