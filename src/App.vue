<script setup>
import NavbarComponent from './components/NavbarComponent.vue'
import HeroComponent from './components/HeroComponent.vue'
import AboutComponent from './components/AboutComponent.vue'
import ServicesComponent from './components/ServicesComponent.vue'
import TeamComponent from './components/TeamComponent.vue'
import FooterComponent from './components/FooterComponent.vue'

</script>

<template>
  <NavbarComponent />
  
  <section id="home"><HeroComponent /></section>
  <section id="about"><AboutComponent /></section>
  <section id="services"><ServicesComponent /></section>
  <section id="team"><TeamComponent /></section>
  <section id="contact"><FooterComponent /></section>
</template>

<style>
html {
  scroll-behavior: smooth; 
}
</style>