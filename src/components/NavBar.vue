<script setup>
import Gong from '@/assets/img.svg'
import Header from './Header.vue'
</script>

<template>
  <!-- ANNOUCEMENT -->
  <div class="container">
    <div class="annouce">
      <img :src="Gong" alt="announcement icon" />
      <span>NEW PROGRAM ALERT</span>
      <div class="capt">
        Get measureable results fast with our proven methods
        <p class="btn-action">Explore →</p>
      </div>
      <div class="close">×</div>
    </div>
  </div>
  <Header />
</template>

<style scoped>
.annouce {
  color: #fff;
  max-width: 1200px;
  position: relative;
  width: 100%;
  padding: 1rem 0;
  font-size: 12px;
}

.capt {
  max-width: 250px;
}

.annouce img,
.annouce span {
  display: none;
}

.btn-action {
  cursor: pointer;
  display: inline;
  font-weight: 600;
}

.close {
  border: 1px solid #fff;
  border-radius: 50%;
  width: 28px;
  height: 28px;
  display: grid;
  place-items: center;
  cursor: pointer;
  position: absolute;
  top: 50%;
  right: calc(5px / 2);
  transform: translate(-50%, -50%);
}

@media (min-width: 750px) {
  .annouce {
    display: flex;
    gap: 24px;
    align-items: center;
    justify-content: center;
  }

  .capt {
    min-width: fit-content;
  }

  .annouce img,
  .annouce span {
    display: flex;
  }

  .capt p {
    margin-left: 24px;
  }
}
</style>
