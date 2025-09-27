<script setup>
import MenuIcon from '@/assets/BtnImage.svg'
import PryBtn from './PryBtn.vue'
import Logo from './Logo.vue'
</script>
<template>
  <header>
    <div class="container">
      <div class="head">
        <Logo />
        <nav>
          <ul>
            <li>Consulting</li>
            <li>Program</li>
            <li>Platfrom</li>
            <li>Pricing</li>
            <li>Resources</li>
          </ul>
          <PryBtn txt="Talk to us" :isIcon="false" />
        </nav>
        <img :src="MenuIcon" class="menu-icon" alt="logo" />
      </div>
    </div>
  </header>
</template>
<style scoped>
header {
  background-color: var(--background-blue);
}

.head {
  width: 100%;
  display: flex;
  justify-content: space-between;
  /* padding: 0 20px; */
}

.menu-icon {
  width: 100px;
  margin-right: -20px;
}

nav ul li {
  padding: 18px 9px;
  cursor: pointer;
}

nav {
  display: none;
  align-items: center;
  justify-content: center;
}

@media (min-width: 750px) {
  nav {
    display: flex;
  }

  nav ul {
    display: flex;
    list-style-type: none;
    gap: 10px;
    padding: 14px 9px;
  }

  .menu-icon {
    display: none;
  }
}
</style>
