<script setup>
import PryBtn from './PryBtn.vue'
import quote from '@/assets/quote.svg'
</script>
<template>
  <section>
    <div class="container">
      <div>
        <div class="head">
          <h4>ABOUT US</h4>
          <h3>Our methods have been endorsed by ambitious companies and innovators worldwide</h3>
          <PryBtn txt="Read our story" :isIcon="true" />
        </div>

        <div class="cards">
          <div class="card">
            <h3 class="pink">#1</h3>
            <span>Most popular tool to learn innovation & entrepreneurship</span>
          </div>
          <div class="card">
            <h3 class="pink">200k+</h3>
            <span>Companies guided by Strategyzer frameworks</span>
          </div>
          <div class="card">
            <h3 class="pink">Top 10</h3>
            <span>Most cited business book of all time (Financial Times)</span>
          </div>
          <div class="card">
            <h3 class="pink">178+</h3>
            <span>Countries where our processes help empower teams</span>
          </div>
        </div>

        <div class="quote">
          <img :src="quote" alt="quote" />
          <h2>
            With disruption around every corner corporate leaders need to think about business
            models as a strategic weapon. Strategyzer will help your company stay and win in
            business.”
          </h2>
          <div class="founder">
            <span>Steve Blank</span>
            <p>The Father of Modern Entrepreneurship</p>
          </div>
        </div>
      </div>
    </div>
    <div class="hidden">
      <div class="cyan"></div>
      <div class="blue"></div>
    </div>
  </section>
</template>
<style scoped>
section {
  width: 100%;
  background-color: #0026df;
}

.container > div {
  padding: 60px 30px 60px;
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

.cyan {
  height: 100px;
  width: 480px;
  background-color: #4dced4;
}

.blue {
  height: 100px;
  flex: 1;
  background-color: #0026df;
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
  padding-bottom: 50px;
}

.card {
  flex: 1;
  min-width: 340px;
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 15px;
  text-align: center;
}

.card h3 {
  color: #ff58f9;
  font-weight: 400;
  font-size: 48px;
  line-height: 57.6px;
  letter-spacing: 0%;
}

.card span {
  font-weight: 300;
  font-size: 14px;
  line-height: 16.8px;
  letter-spacing: 0%;
}

h2 {
  font-weight: 300;
  font-size: 28px;
  line-height: 33.6px;
  letter-spacing: -0.84px;
  margin-bottom: 30px;
  color: #ff58f9;
}

.quote img {
  width: 32px;
  height: 28px;
  margin-bottom: 31px;
}

.founder span {
  font-weight: 500;
  font-style: Medium;
  font-size: 14px;
  line-height: 16.8px;
  letter-spacing: 0%;
  color: #fff;
}

.founder p {
  color: #ff58f9;
  font-weight: 500;
  font-style: Medium;
  font-size: 14px;
  line-height: 16.8px;
  letter-spacing: 0%;
  vertical-align: middle;
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
    max-width: 880px;
  }

  .cards {
    justify-content: space-between;
    padding-bottom: 120px;
  }

  .card {
    flex: 1;
    min-width: 210px;
    max-width: 220px;
  }

  .card h3 {
    font-size: 72px;
    line-height: 86.4px;
    letter-spacing: 0%;
  }

  .card span {
    font-size: 22px;
    line-height: 26.4px;
    letter-spacing: 0%;
    text-align: left;
  }

  h2 {
    font-weight: 300;
    font-size: 52px;
    line-height: 62.4px;
    letter-spacing: -1.56px;
    margin-bottom: 31px;
  }

  .quote img {
    width: 50px;
    height: 38px;
    margin-bottom: 31px;
  }

  .founder span {
    font-size: 22px;
    line-height: 26.4px;
    letter-spacing: 0%;
  }

  .founder p {
    font-size: 22px;
    line-height: 26.4px;
    letter-spacing: 0%;
  }
}
</style>
