<script setup>
import PryBtn from './PryBtn.vue'
import CONSULTING from '@/assets/CONSULTING.png'
import PROGRAMS from '@/assets/PROGRAMS.png'
</script>
<template>
  <section>
    <div class="container">
      <div>
        <div class="head">
          <h4>WHAT WE DO</h4>
          <h3>Innovate smarter guided by our expertise</h3>
        </div>

        <div class="cards">
          <div class="card">
            <div class="card-head">
              <img :src="PROGRAMS" alt="" />
              <h3>Programs</h3>
            </div>
            <span
              >Derisk ideas and achieve results quickly with proven processes, guided workflow and
              expert support. Make innovation practical for everyone in your team.</span
            >
            <PryBtn txt="Find out more" BtnColor="#fff" :isIcon="true" />
          </div>
          <div class="card">
            <div class="card-head">
              <img :src="CONSULTING" alt="" />
              <h3>Consulting</h3>
            </div>
            <span
              >Transform the way strategy, growth and innovation is viewed, measured and delivered
              in your business. Build forward-looking capabilities in every team to tackle any
              challenge.</span
            >
            <PryBtn txt="Find out more" BtnColor="#fff" :isIcon="true" />
          </div>
        </div>
      </div>
    </div>
    <div class="hidden">
      <div class="blue"></div>
      <div class="black"></div>
    </div>
  </section>
</template>
<style scoped>
section {
  width: 100%;
}

.head {
  min-width: 170px;
  width: 100%;
  padding-right: 90px;
  display: flex;
  flex-direction: column;
  gap: 19px;
  margin-bottom: 40px;
}

.container > div {
  padding: 60px 30px 60px;
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

.blue {
  height: 100px;
  width: 480px;
  background-color: #0026df;
}

.black {
  height: 100px;
  flex: 1;
  background-color: #000;
}

h3 {
  font-size: 28px;
  line-height: 28px;
  letter-spacing: -0.84px;
}

h4 {
  font-size: 12px;
  line-height: 13.2px;
  letter-spacing: 0.72px;
}

.cards {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  gap: 30px;
}

.card {
  flex: 1;
  min-width: 200px;
  max-width: 550px;
  display: flex;
  flex-direction: column;
  gap: 35px;
}

.card-head {
  display: flex;
  align-items: start;
  flex-direction: column;
  gap: 16px;
}

.card-head img {
  width: 129px;
  height: 128px;
  object-fit: contain;
  object-position: center;
}

span {
  font-weight: 300;
  font-style: Regular;
  font-size: 18px;
  line-height: 24.6px;
  letter-spacing: -0.36px;
}

@media (min-width: 750px) {
  h3 {
    font-size: 52px;
    line-height: 52px;
    letter-spacing: -1.56px;
  }

  h4 {
    font-size: 16px;
    line-height: 17.6px;
    letter-spacing: 0.96px;
  }

  .hidden {
    display: flex;
  }

  .head {
    margin-bottom: 120px;
    max-width: 640px;
  }

  .card-head {
    gap: 48px;
    flex-direction: row;
    align-items: center;
  }

  .card-head img {
    width: 180px;
    height: 180px;
  }

  span {
    font-weight: 300;
    font-size: 28px;
    line-height: 39.2px;
    letter-spacing: -0.5px;
  }
}
</style>
