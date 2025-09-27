<script setup>
import IBL from '@/assets/278ef3a419ee93c8d6f8e4fd8477793a9ef50c28.png'
import biozyme from '@/assets/f71754ba9cb476a9b1bb4abde0a7854611f8af4e.png'
import IIpic from '@/assets/3107226d2a0f34a8d01441fb2acc9749394d9957.png'
import bayer from '@/assets/64d5006e78bc9838711b8f8f_Logo.svg.png'
import accelerator from '@/assets/65aa42ac3ddcc0abf6adcedd_pharma.svg fill.png'
import msd from '@/assets/msdlogo.png'
import cyric from '@/assets/cyric.png'
import schreiber from '@/assets/SVG (2).png'
import mastercardlogo from '@/assets/mastercardlogo.png'
import Bovedalogo from '@/assets/Bovedalogo.png'
import Ah from '@/assets/2c697d646d700caee1c21afbfb95ecfa60904445.png'
import PryBtn from './PryBtn.vue'
</script>
<template>
  <section>
    <div class="grid-container">
      <div class="grid">
        <div class="box box1">
          <img :src="IBL" alt="ibl" />
          <div>
            <span>Build resilience and innovate autonomously with guided programs.</span>
            <PryBtn :isIcon="true" BtnColor="#471169" />
          </div>
        </div>
        <div class="box box2">
          <img :src="biozyme" alt="ibl" />
          <div>
            <span
              >Many companies provide innovation tools, theoretical knowledge, and training
              programs. What sets Strategyzer apart is the way they blend all these elements into an
              actionable format. This approach helps you take concrete steps and start doing, rather
              than wasting valuable time figuring out how to begin.</span
            >
            <div class="profile">
              <img :src="IIpic" alt="" />
              <div class="profile-details">
                <span class="name">Ignacio Ipharraguerre</span>
                <span class="position">VP Research & Innovation</span>
              </div>
            </div>
          </div>
        </div>
        <div class="box box3">
          <img :src="bayer" alt="ibl" />
          <div>
            <span>Build an innovation system to produce 1 billion in new revenue.</span>
            <PryBtn :isIcon="true" BtnColor="#0026DF" />
          </div>
        </div>
        <div class="box box4">
          <img :src="accelerator" alt="ibl" />
          <div>
            <span>Building a successful innovation accelerator to change lives.</span>
            <PryBtn :isIcon="true" BtnColor="#471169" />
          </div>
        </div>
        <div class="box box5">
          <img :src="msd" alt="ibl" />
          <div>
            <span>Enabling world-wide access to life saving technologies.</span>
            <PryBtn :isIcon="true" BtnColor="#4DCED4" />
          </div>
        </div>
        <div class="box box6">
          <img :src="cyric" alt="ibl" />
          <div>
            <span
              >Thanks to Strategyzer, we’ve been able to acquire proven methods and established
              innovation management processes fast, so we didn’t have to reinvent everything from
              scratch.</span
            >
            <div class="profile">
              <img :src="Ah" alt="" />
              <div class="profile-details">
                <span class="name">Antonis Hadjiantonis</span>
                <span class="position">Innovation Directors</span>
              </div>
            </div>
          </div>
        </div>
        <div class="box box7">
          <img :src="schreiber" alt="ibl" />
          <div>
            <span
              >Proving the value of innovation and rekindling a company-wide culture to support
              it.</span
            >
            <PryBtn :isIcon="true" BtnColor="#471169" />
          </div>
        </div>
        <div class="box box8">
          <img :src="mastercardlogo" alt="ibl" />
          <div>
            <span>Unify a global workforce through a shared language of innovation.</span>
            <PryBtn :isIcon="true" BtnColor="#EB2835" />
          </div>
        </div>
        <div class="box box9">
          <img :src="Bovedalogo" alt="ibl" />
          <div>
            <span
              >Thanks to Strategyzer, we’ve been able to acquire proven methods and established
              innovation management processes fast, so we didn’t have to reinvent everything from
              scratch.</span
            >
            <div class="flex">
              <div class="profile">
                <img :src="Ah" alt="" />
                <div class="profile-details">
                  <span class="name">Antonis Hadjiantonis</span>
                  <span class="position">Innovation Directors</span>
                </div>
              </div>
              <PryBtn :isIcon="true" BtnColor="#0026df" />
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="hidden">
      <div class="yellow"></div>
      <div class="black"></div>
    </div>
  </section>
</template>
<style scoped>
section {
  width: 100%;
  background-color: #000;
  padding: 0 10px 60px;
}
.flex {
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.hidden {
  display: none;
  max-width: 1440px;
  margin: 0 auto;
}

.profile {
  display: flex;
  gap: 10px;
  width: fit-content;
  font-size: 16px;
  line-height: 22.4px;
  align-items: center;
}

.profile img {
  width: 70px;
  height: 70px;
}

.profile-details {
  display: flex;
  flex-direction: column;
  gap: 5px;
}

.profile-details span {
  width: max-content;
}

.yellow {
  height: 100px;
  width: 480px;
  background-color: #ffd642;
}

.black {
  height: 100px;
  flex: 1;
  background-color: #000;
}

.grid-container {
  max-width: 1440px;
  margin: 0 auto;
  display: flex;
  justify-content: center;
  align-items: center;
}

.grid {
  display: grid;
  grid-template-columns: 1fr; /* Mobile first: single column */
  grid-auto-rows: auto;
  width: 100%;
}

.box {
  width: 100%;
  height: 100%;
  padding: 32px 20px;
  display: flex;
  flex-direction: column;
  gap: 25px;
  justify-content: space-between;
}

.box > img {
  height: 50px;
  width: 100%;
  object-fit: contain;
  object-position: left;
}

.box > div {
  display: flex;
  flex-direction: column;
  gap: 25px;
}

.box > div > span {
  font-weight: 400;
  font-style: Regular;
  font-size: 18px;
  line-height: 21.6px;
  letter-spacing: -0.36px;
}

.box1 {
  background: #4dced4;
  color: #471169;
}

.box2 {
  background: #ffd642;
  color: #eb2835;
}

.box3 {
  background: #74be47;
  color: #0026df;
}
.box4 {
  background: #ff58f9;
  color: #471169;
}
.box5 {
  background: #471169;
  color: #4dced4;
}
.box6 {
  background: #0026df;
  color: #4dced4;
}
.box7 {
  background: #eb2835;
  color: #471169;
}
.box8 {
  background: #ffd642;
  color: #eb2835;
}
.box9 {
  background: #74be47;
  color: #0026df;
}

@media (min-width: 750px) {
  .grid {
    grid-template-columns: repeat(6, 1fr);
    grid-auto-rows: 480px;
  }

  /* Row 1 */
  .box1,
  .box3,
  .box4,
  .box5,
  .box7,
  .box8 {
    grid-column: span 2;
  }
  .box2,
  .box6,
  .box9 {
    grid-column: span 4;
  }

  .hidden {
    display: flex;
  }

  .box > div > span {
    font-weight: 400;
    font-size: 28px;
    line-height: 39.2px;
    letter-spacing: -0.5px;
  }

  .box > span {
    font-size: 32px;
    line-height: 38.4px;
    letter-spacing: -0.64px;
  }

  .box > img {
    height: 120px;
  }

  section {
    padding: 0;
  }
}
</style>
