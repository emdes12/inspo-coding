<script setup>
import teams from '@/assets/Container.png'
import Submit from './Submit.vue'

const formCLick = (e) => {
  e.preventDefault()
  alert('Thanks you for reaching out')
}
</script>

<template>
  <section>
    <div class="container">
      <div class="flex">
        <img :src="teams" alt="teams image" />
        <div class="contact-sect">
          <h1>Connect with our team about your business goals</h1>
          <span
            >Reach out about pricing, a demo, or team enrollment. We’ll be in touch shortly!</span
          >

          <form :action="formCLick">
            <div class="form-group">
              <input type="text" placeholder="First Name*" required />
              <input type="text" placeholder="Last Name*" required />
            </div>
            <input type="email" placeholder="Work email*" required />
            <input type="text" placeholder="What's you job title?" />
            <input type="text" placeholder="What best describes you?*" required />
            <select name="describe" id="desc">
              <option value="">What best describes you?*</option>
              <option value="inspired">Self Motivator</option>
            </select>
            <select name="describe" id="desc">
              <option value="">What are you inquiring about?*</option>
              <option value="inspired">How to buy and sell</option>
            </select>
            <textarea
              name="message"
              id="mess"
              required
              placeholder="Tell us about your needs and goals? How can we help you?*"
            ></textarea>
            <input type="text" placeholder="How did you hear about us?*" required />
            <p>Have questions or different needs? Reach out to us <a href="#">here</a></p>
            <Submit txt="Speak with an expert" />
          </form>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
form {
  display: flex;
  flex-direction: column;
  gap: 30px;
}

input,
select,
textarea {
  border: none;
  border-radius: 16px;
  padding: 18px 25px;
  width: 100%;
  font-size: 1rem;
}

p {
  font-size: 14px;
  line-height: 16px;
}

.form-group {
  display: flex;
  gap: 30px;
}

select {
  color: #666;
}

a {
  text-decoration: underline;
  color: #fff;
}

section {
  width: 100%;
  background-color: #0026df;
}

.container {
  max-width: 1440px;
  padding: 0;
}

.contact-sect {
  width: 100%;
  padding: 20px;
  display: flex;
  flex-direction: column;
}

.contact-sect h1 {
  font-size: 32px;
  line-height: 35.2px;
  letter-spacing: 0%;
  color: #ffd642;
}

.contact-sect span {
  font-size: 18px;
  line-height: 25.2px;
  letter-spacing: 0%;
  padding-top: 40px;
  padding-bottom: 50px;
}

.grid {
  display: grid;
  grid-template-columns: 1fr;
}

img {
  display: none;
}
@media (min-width: 1000px) {
  .grid {
    grid-template-columns: 1fr 1fr;
  }

  img {
    display: flex;
  }
}

@media (min-width: 750px) {
  .contact-sect {
    padding: 64px;
  }

  .contact-sect h1 {
    font-size: 58px;
    line-height: 63.8px;
  }

  .contact-sect span {
    font-size: 30px;
    line-height: 42px;
    padding-bottom: 83px;
  }
}
</style>
