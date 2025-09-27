<script setup>
import logo from '@/assets/Link - home.svg'
</script>
<template>
  <img :src="logo" class="logo" alt="logo" />
</template>
<style scoped>
.logo {
  width: 140px;
}

@media (min-width: 750px) {
  .logo {
    width: 210px;
  }
}
</style>
