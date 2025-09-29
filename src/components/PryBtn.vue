<script setup>
import Arrow from '@/assets/SVG (1).svg'

defineProps({
  txt: {
    type: String,
    required: true,
  },
  isIcon: {
    type: Boolean,
    required: false,
    default: false,
  },
  BtnColor: {
    type: String,
    default: '#fff',
    required: false,
  },
  notActive: {
    type: Boolean,
    default: false,
    required: false,
  },
  isLeft: {
    type: Boolean,
    default: false,
    required: false,
  },
})
</script>
<template>
  <button
    class="with-text"
    v-if="txt && !notActive"
    :style="{ color: BtnColor, borderColor: BtnColor }"
  >
    {{ txt }}
    <svg
      v-if="isIcon"
      width="25"
      height="25"
      viewBox="0 0 25 25"
      fill="none"
      xmlns="http://www.w3.org/2000/svg"
    >
      <path
        d="M13.909 2.62L23.1701 12.3333L13.909 21.82M1.42896 12.22H22.549"
        :stroke="BtnColor"
        stroke-width="1.92"
      />
    </svg>
  </button>
  <button
    class="without-text"
    v-if="!txt && !notActive"
    :style="{ color: BtnColor, borderColor: BtnColor }"
  >
    <!-- {{ txt }} -->
    <svg
      v-if="isIcon"
      width="25"
      height="25"
      viewBox="0 0 25 25"
      fill="none"
      xmlns="http://www.w3.org/2000/svg"
    >
      <path
        d="M13.909 2.62L23.1701 12.3333L13.909 21.82M1.42896 12.22H22.549"
        :stroke="BtnColor"
        stroke-width="1.92"
      />
    </svg>
  </button>
  <button
    class="without-text"
    v-if="!txt && notActive && !isLeft"
    :style="{ color: BtnColor, borderColor: BtnColor, opacity: '40%' }"
  >
    <!-- {{ txt }} -->
    <svg
      v-if="isIcon"
      width="25"
      height="25"
      viewBox="0 0 25 25"
      fill="none"
      xmlns="http://www.w3.org/2000/svg"
    >
      <path
        d="M13.909 2.62L23.1701 12.3333L13.909 21.82M1.42896 12.22H22.549"
        :stroke="BtnColor"
        stroke-width="1.92"
      />
    </svg>
  </button>
  <button
    class="without-text"
    v-if="!txt && notActive && isLeft"
    :style="{ color: BtnColor, borderColor: BtnColor, transform: 'rotate(180deg)', opacity: '40%' }"
  >
    <!-- {{ txt }} -->
    <svg
      v-if="isIcon"
      width="25"
      height="25"
      viewBox="0 0 25 25"
      fill="none"
      xmlns="http://www.w3.org/2000/svg"
    >
      <path
        d="M13.909 2.62L23.1701 12.3333L13.909 21.82M1.42896 12.22H22.549"
        :stroke="BtnColor"
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
  background-color: transparent;
  border: 2px solid #fff;
  padding: 13px 23px;
  color: #fff;
  font-weight: 300;
  border-radius: 96px;
  cursor: pointer;
  font-weight: 400;
  line-height: 19.5px;
  letter-spacing: 0.13px;
}

.without-text {
  border: none;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 10px;
  width: fit-content;
  background-color: transparent;
  border: 2px solid #fff;
  width: 45px;
  height: 45px;
  border-radius: 50%;
  color: #fff;
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

@media (min-width: 750px) {
  .without-text {
    width: 60px;
    height: 60px;
  }
}
</style>
