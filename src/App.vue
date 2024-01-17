<script setup>
import Navigation from './components/Navigation.vue'
import Hero from './components/Hero.vue'
import TextSection from './components/TextSection.vue'
import ListObject from './components/ListObject.vue'
import Prijzen from './components/Tarieven.vue'
import FooterSection from './components/Footer.vue'
</script>

<template>
  <Navigation />

  <main>
    <Hero />
    <TextSection title="Midden in de Natuur" title2='Duurzaam'/>
    <ListObject />
    <Prijzen />
  </main>

  <FooterSection/>
</template>
