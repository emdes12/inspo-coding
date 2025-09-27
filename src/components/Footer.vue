<script setup>
import Logo from './Logo.vue'
import PryBtn from './PryBtn.vue'
</script>
<template>
  <section>
    <div class="section">
      <div class="business-info">
        <Logo />
        <p>Outcomes Driven Business Programs & Consulting Solutions</p>
        <PryBtn txt="talk to us" />
      </div>

      <div class="links">
        <div class="link-container">
          <div class="link-head">Contact Us</div>
          <div class="link-group">
            <p>Strategyzer AG, Zone Industrielle (ZI) Le Tresi 9B1028 Préverenges, Switzerland</p>
            <a href="#">LinkedIn</a>
          </div>
        </div>
        <div class="link-container">
          <div class="link-head">Programs</div>
          <ul class="link-group">
            <li><a href="#">Innovation Programs</a></li>
            <li><a href="#">Strategy Programs</a></li>
            <li><a href="#">Marketing Programs</a></li>
            <li><a href="#">Program Library</a></li>
          </ul>
        </div>
        <div class="link-container">
          <div class="link-head">Products</div>
          <ul class="link-group">
            <li><a href="#">Programs & Training</a></li>
            <li><a href="#">Consulting & Advisory</a></li>
            <li><a href="#">Platforms</a></li>
          </ul>
        </div>
        <div class="link-container">
          <div class="link-head">Resources</div>
          <ul class="link-group">
            <li><a href="#">Insights</a></li>
            <li><a href="#">Webinars</a></li>
            <li><a href="#">White Papers</a></li>
            <li><a href="#">Case Studies</a></li>
            <li><a href="#">Events</a></li>
            <li><a href="#">Self-Paced Trainings</a></li>
          </ul>
        </div>
        <div class="link-container">
          <div class="link-head">Company</div>
          <ul class="link-group">
            <li><a href="#">About Us</a></li>
            <li><a href="#">Contact Us</a></li>
            <li><a href="#">Team</a></li>
          </ul>
        </div>
        <div class="link-container">
          <div class="link-head">Platform Account</div>
          <ul class="link-group">
            <li><a href="#">Sign up</a></li>
            <li><a href="#">Login in</a></li>
          </ul>
        </div>
        <div class="link-container">
          <div class="link-head">Top Content</div>
          <ul class="link-group">
            <li><a href="#">Business Model Canvas</a></li>
            <li><a href="#">Value Proposition</a></li>
            <li><a href="#">Tools & Download</a></li>
            <li><a href="#">Book</a></li>
          </ul>
        </div>
        <div class="link-container">
          <div class="link-head hide">Top Content</div>
          <ul class="link-group">
            <li><a href="#">Business Model Generations</a></li>
            <li><a href="#">Value Proposition Design</a></li>
            <li><a href="#">Invincible Companies</a></li>
            <li><a href="#">Testing Business</a></li>
          </ul>
        </div>
      </div>

      <div class="copyrights">
        <div class="name">Copyright {{ year }} - Strategyzer AG</div>
        <div class="divd">|</div>
        <a href="#" class="foot">Terms of Service</a>
        <div class="divd">|</div>
        <a href="#" class="foot">Privacy Policy</a>
        <div class="divd">|</div>
        <a href="#" class="foot">Copyright & IP Policy</a>
      </div>
    </div>
  </section>
</template>
<style scoped>
.hide {
  display: none;
  visibility: hidden;
}

a {
  color: inherit;
  text-decoration: none;
  cursor: pointer;
}

section {
  width: 100%;
}

.section {
  color: #fff;
  background-color: #000;
  padding: 60px 30px 60px;
  max-width: 1440px;
  margin: 0 auto;
  width: 100%;
  display: flex;
  flex-wrap: wrap;
  flex-direction: column;
  gap: 30px;
}

.link-group {
  display: flex;
  flex-direction: column;
  gap: 20px;
  color: #959ca3;
  font-size: 12px;
  line-height: 18px;
  list-style-type: none;
  padding-top: 20px;
}

.link-head {
  text-transform: uppercase;
}

.business-info {
  max-width: 280px;
  width: 100%;
  display: flex;
  flex-direction: column;
  gap: 20px;
}

.links {
  flex: 1;
  display: flex;
  flex-wrap: wrap;
  gap: 30px;
}

.link-container {
  max-width: 220px;
  min-width: 220px;
}

.name {
  color: #959ca3;
}

.copyrights {
  display: flex;
  align-items: start;
  flex-direction: column-reverse;
  gap: 20px;
  width: 100%;
  padding-top: 20px;
}

a.foot {
  color: #fff;
}

.divd {
  display: none;
}

@media (min-width: 750px) {
  .section {
    flex-direction: row;
    gap: 100px;
  }

  .hide {
    display: flex;
  }

  .copyrights {
    align-items: center;
    justify-content: center;
    flex-direction: row;
    gap: 30px;
  }

  .divd {
    display: flex;
  }
}
</style>
