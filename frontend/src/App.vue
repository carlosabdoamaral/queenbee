<script setup lang="ts">
import Hero from "./components/home/Hero.vue";
import Quote from "./components/home/Quote.vue";
import Products from "./components/home/Products.vue"
import About from "./components/home/About.vue";
import Header from "./components/home/Header.vue";
import Contact from "./components/home/Contact.vue";
import Footer from "./components/home/Footer.vue";
</script>

<template>
  <main>
    <div class="main-wrapper">
      <Hero />
      <Header />

      <div style="height: 20dvh;"></div>
      <Quote />

      <div style="height: 20dvh;" id="about"></div>
      <About />

      <div style="height: 20dvh;" id="products"></div>
      <Products />

      <div style="height: 20dvh;" id="contact"></div>
      <Contact />

      <div style="height: 10dvh;" id="contact"></div>
      <Footer />
    </div>
  </main>
</template>

<style lang="scss" scoped>
$heroHeight: 50dvh;
$accent: #ffc400;
$comp: #3c2300;
</style>
