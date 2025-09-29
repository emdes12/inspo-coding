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

svg {
  transition: all 0.5s ease-in-out;
}

button {
  cursor: pointer;
}

svg {
  width: 24px;
  height: 24px;
}

button:hover {
  background-color: #0000005d;
}

button:hover svg {
  animation: swing 1s ease-in-out infinite;
}

@keyframes swing {
  0% {
    transform: translateX(5px);
    color: red;
  }

  100% {
    transform: translateX(-5px);
    color: chocolate;
  }
}
</style>
