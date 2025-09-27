<script setup>
import trustee from '@/assets/trustees/trustee (1).png'
import trustee2 from '@/assets/trustees/trustee (2).png'
import trustee3 from '@/assets/trustees/trustee (3).png'
import trustee4 from '@/assets/trustees/trustee (4).png'
import trustee5 from '@/assets/trustees/trustee (5).png'
import trustee6 from '@/assets/trustees/trustee (6).png'
import trustee7 from '@/assets/trustees/trustee (7).png'
import trustee8 from '@/assets/trustees/trustee (8).png'
import trustee9 from '@/assets/trustees/trustee (9).png'
import PryBtn from './PryBtn.vue'
</script>

<template>
  <section>
    <div class="container">
      <div class="trustee">
        <h4>TRUSTED BY THE WORLD'S OST AMIBITIOUS COMPANIES</h4>
        <div class="trustees-logo">
          <img :src="trustee" alt="logos" />
          <img :src="trustee2" alt="logos" />
          <img :src="trustee3" alt="logos" />
          <img :src="trustee4" alt="logos" />
          <img :src="trustee5" alt="logos" />
          <img :src="trustee6" alt="logos" />
          <img :src="trustee7" alt="logos" />
          <img :src="trustee8" alt="logos" />
          <img :src="trustee9" alt="logos" />
          <img :src="trustee" alt="logos" />
          <img :src="trustee" alt="logos" />
          <img :src="trustee" alt="logos" />
        </div>

        <div class="aim-obj">
          <div class="objective">
            <h3>
              We guide companies to build innovation capabilities across all departments and roles
            </h3>
            <PryBtn txt="Read case studies" :is-icon="true" BtnColor="#000" />
          </div>
        </div>
      </div>
    </div>
    <div class="hidden">
      <div class="cyan"></div>
      <div class="white"></div>
    </div>
  </section>
</template>

<style scoped>
.hidden {
  display: none;
  max-width: 1440px;
  margin: 0 auto;
}

.cyan {
  height: 100px;
  width: 480px;
  background-color: #4dced4;
}

.white {
  height: 100px;
  flex: 1;
  background-color: #fff;
}

section {
  background-color: #fff;
  color: #959ca3;
  padding-top: 70px;
}

h3 {
  font-size: 28px;
  line-height: 33.6px;
  letter-spacing: -0.84px;
}

h4 {
  font-size: 12px;
  line-height: 13.2px;
  letter-spacing: 0.72px;
}

.aim-obj {
  display: flex;
  justify-content: end;
}

.objective {
  display: flex;
  flex-direction: column;
  gap: 25px;
  max-width: 768px;
  width: 100%;
  color: #000;
}

.trustees-logo {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 20px;
  flex-wrap: wrap;
}

img {
  width: 70px;
  height: 44px;
  object-position: center;
  object-fit: contain;
}

.trustee {
  display: flex;
  flex-direction: column;
  gap: 67px;
  padding-bottom: 70px;
}

@media (min-width: 750px) {
  .trustee {
    gap: 100px;
  }

  .hidden {
    display: flex;
  }

  h3 {
    font-size: 52px;
    line-height: 62.4px;
    letter-spacing: -1.56px;
  }

  h4 {
    font-size: 16px;
    line-height: 17.6px;
    letter-spacing: 0.96px;
  }

  .objective {
    gap: 48px;
  }
}
</style>
