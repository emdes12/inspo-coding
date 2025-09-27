<script setup>
import HeroImage from '@/assets/Img.png'
import PryBtn from './PryBtn.vue'
</script>
<template>
  <section>
    <div class="container">
      <div class="hero-section">
        <img :src="HeroImage" class="hero-img" alt="hero-img" />
        <div class="hero-capt">
          <h2>Drive strategy, align teams, and grow winning ideas</h2>
          <span>
            Craft strategy, grow, and build resilience with our expert team. Create more customer
            and company value with our hands-on programs. For sales, marketing, product &
            innovation.
          </span>
          <div class="hero-action">
            <PryBtn txt="Get Started" :is-icon="true" BtnColor="#fff" />
            <PryBtn txt="Speak to us" :is-icon="true" BtnColor="#fff" />
          </div>
          <p>No credit card required. upgrade any time</p>
        </div>
      </div>
    </div>
    <div class="empty-white"></div>
  </section>
</template>
<style scoped>
h2 {
  font-size: 50px;
  line-height: 55px;
  letter-spacing: -1.5px;
  color: var(--color-purple);
}

.empty-white {
  width: 100%;
  height: 40px;
  background-color: #fff;
}

.hero-capt {
  min-width: 270px;
  flex: 1;
  padding-right: 120px;
  display: flex;
  flex-direction: column;
  align-items: start;

  z-index: 100000;
}

section {
  background-color: var(--background-blue);
  width: 100%;
  overflow: hidden;
  position: relative;
}

.hero-section {
  position: relative;
  padding: 50px 0 80px;
  display: flex;
  flex-direction: row-reverse;
  width: 100%;
  align-items: end;
}

.hero-action {
  display: flex;
  gap: 1rem;
  padding-top: 20px;
  flex-direction: column;
  padding-bottom: 14px;
}

.hero-img {
  width: 280px;
  height: 370px;
  z-index: 1;
  /* margin: -200px; */
  /* padding-right:; */
  position: absolute;
  bottom: -40px;
}

span {
  font-weight: 400;
  font-style: Regular;
  font-size: 18px;
  line-height: 25.2px;
  vertical-align: middle;
  padding-top: 1rem;
  padding-bottom: 42px;
}

@media (min-width: 750px) {
  .hero-section {
    width: 100%;
    display: flex;
    flex-direction: row-reverse;
    align-items: start;
    /* padding-bottom: 50px; */
  }

  h2 {
    font-size: 74px;
    line-height: 81.4px;
    /* width: 100%; */
  }

  .hero-capt {
    flex: 1;
  }

  .hero-img {
    position: static;
    height: 735px;
    width: 540px;
    margin: 0;
    margin-right: -100px;
  }

  .hero-action {
    flex-direction: row;
    width: 100%;
  }

  .empty-white {
    width: 70%;
    position: absolute;
    height: 100px;
    bottom: 0;
    left: 0;
    background-color: #fff;
  }
}
</style>
