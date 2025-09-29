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
  <button class="with-text" type="submit">
    {{ txt }}
    <svg width="25" height="25" viewBox="0 0 25 25" fill="none" xmlns="http://www.w3.org/2000/svg">
      <path
        d="M13.909 2.62L23.1701 12.3333L13.909 21.82M1.42896 12.22H22.549"
        stroke="#fff"
        stroke-width="1.92"
      />
    </svg>
  </button>
</template>
<style scoped>
.with-text {
  border: none;
  display: flex;
  align-items: center;
  gap: 10px;
  width: fit-content;
  background-color: #000;
  padding: 13px 23px;
  color: #fff;
  font-weight: 300;
  border-radius: 96px;
  cursor: pointer;
  font-weight: 400;
  line-height: 19.5px;
  letter-spacing: 0.13px;
}

svg {
  width: 24px;
  height: 24px;
}

svg {
  transition: all 0.5s ease-in-out;
}

button {
  cursor: pointer;
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
