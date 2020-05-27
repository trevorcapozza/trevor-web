<template>
  <div>
    <div class="hero">
      <AnimatedText/>
    </div>
    <div class="container max">
      <div class="art">
        <img src="@/assets/data.svg" alt="">
        <p>
          4 years experience creating in-depth data reports.
        </p>
      </div>
      <div class="art">
        <img src="@/assets/developer.svg" alt="">
        <p>
          8 years experience UI design and front-end development.
        </p>
      </div>
      <div class="art">
        <img src="@/assets/browser.svg" alt="">
        <p>
          Managed over $750,000 in ad spend during 2019.
        </p>
      </div>
    </div>
    <div class="skills max">
      <h1>Skills</h1>
      <p>Over 7 years of design experience<br>using these programs.</p>
      <div class="programs">
      <img src="@/assets/ps.svg" alt="">
      <img src="@/assets/ai.svg" alt="">
      <img src="@/assets/dw.svg" alt="">
      <img src="@/assets/xd.svg" alt="">
      </div>
    </div>
    <Contact/>
    <Footer/>
  </div>
</template>

<script>
import AnimatedText from '@/components/AnimatedText.vue'
import Contact from '@/components/Contact.vue'
import Footer from '@/components/Footer.vue'

export default {
  name: 'Home',
  components: {
    AnimatedText,
    Contact,
    Footer,
  }
}
</script>


