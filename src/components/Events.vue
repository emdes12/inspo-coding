<script setup>
import PryBtn from './PryBtn.vue'
import hosts from '@/assets/e9daa09b340b639f7e187fda7699b99c6b5d18c6.png'
import SecBtn from './SecBtn.vue'
</script>
<template>
  <section>
    <div class="container">
      <div>
        <div class="flex">
          <div class="head">
            <h4>OUR EVENTS</h4>
            <h3>Curious about what it’s like to work with us? Join one of our upcoming events</h3>
            <PryBtn txt="See all upcoming events" :isIcon="true" BtnColor="#000" />
          </div>

          <div class="navigate">
            <PryBtn :isIcon="true" BtnColor="#000" :isLeft="true" :notActive="true" />
            <PryBtn :isIcon="true" BtnColor="#000" :notActive="true" />
          </div>
        </div>

        <div class="head event">
          <h4>2025</h4>
          <h3 class="event-h">Sep. 10, 2025</h3>
          <div class="card">
            <div class="images">
              <img :src="hosts" alt="" />
            </div>
            <div class="info">
              <div>
                <h5>WEBINARS</h5>
                <h4>Competing on Business Models: AI changed everything and nothing</h4>
                <p>
                  While companies race to implement the latest AI tools, the real competitive
                  advantage lies in building business…
                </p>
              </div>
              <SecBtn txt="Sign up" />
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="hidden">
      <div class="blue"></div>
      <div class="cyan"></div>
    </div>
  </section>
</template>
<style scoped>
.card {
  display: flex;
  flex-direction: column;
  max-width: 880px;
  min-width: 200px;
  width: 100%;
  border-radius: 16px;
  overflow: hidden;
}

.card > div {
  height: 201px;
}

.info {
  padding: 16px;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  background-color: #bceff2;
}

.info h5 {
  color: #000;
  font-size: 10px;
  line-height: 11px;
  letter-spacing: 0.6px;
}

.info h4 {
  font-weight: 400;
  font-size: 20px;
  line-height: 28px;
  letter-spacing: -0.34px;
}

.info p {
  display: none;
  font-size: 18px;
  line-height: 27px;
  letter-spacing: 0%;
  color: #000;
}

.images img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  object-position: center;
}

.event h4 {
  font-size: 12px;
  letter-spacing: 0.72px;
}

.event h3 {
  font-size: 24px;
  line-height: 28.8px;
  letter-spacing: -0.48px;
  color: #000;
  padding-bottom: 12px;
}

.head.event {
  gap: 10px;
}

section {
  width: 100%;
  background-color: #4dced4;
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
  flex-direction: column;
  justify-content: space-between;
}

.navigate {
  display: flex;
  gap: 10px;
  margin-bottom: 40px;
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
  color: #0026df;
}

h4 {
  font-size: 12px;
  line-height: 13.2px;
  letter-spacing: 0.72px;
  color: #000;
}

h2 {
  font-weight: 300;
  font-size: 28px;
  line-height: 33.6px;
  letter-spacing: -0.84px;
  margin-bottom: 30px;
  color: #ff58f9;
}

@media (min-width: 850px) {
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

  .event h3 {
    font-size: 36px;
    line-height: 43.2px;
    letter-spacing: -0.72px;
    padding-bottom: 34px;
  }

  .card {
    flex-direction: row;
  }

  .card > div {
    width: 440px;
    height: 520px;
  }

  .info {
    padding: 40px;
  }

  .info h5 {
    font-size: 13px;
  }

  .info h4 {
    font-size: 28px;
    line-height: 39.2px;
    letter-spacing: -0.48px;
    padding-bottom: 20px;
  }

  .info p {
    display: flex;
  }

  .hidden {
    display: flex;
  }

  .head {
    margin-bottom: 120px;
    max-width: 880px;
  }

  h2 {
    font-weight: 300;
    font-size: 52px;
    line-height: 62.4px;
    letter-spacing: -1.56px;
    margin-bottom: 31px;
  }

  .flex {
    flex-direction: row;
    align-items: flex-end;
  }

  .navigate {
    margin-bottom: 120px;
  }
}
</style>
