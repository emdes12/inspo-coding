<script setup>
import logo from '@/assets/Link - home.svg'
import MenuIcon from '@/assets/BtnImage.svg'
import PryBtn from './PryBtn.vue'
</script>
<template>
  <header>
    <div class="container">
      <div class="head">
        <img :src="logo" class="logo" alt="logo" />
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
.logo {
  width: 140px;
}

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
  .logo {
    width: 210px;
  }

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
