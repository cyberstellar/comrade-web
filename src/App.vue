<script setup>
import Header from '@/components/Header.vue'
import Intro from '@/components/Intro.vue'
import OurServices from '@/components/OurServices.vue'
import Gallery from '@/components/Gallery.vue'
import StarIcon from '@/assets/icons/StarIcon.vue'
import Testimonials from '@/components/Testimonials.vue'
import ContactForm from '@/components/ContactForm.vue'
import Footer from '@/components/Footer.vue'
import Benefits from '@/components/Benefits.vue'
</script>

<template>
  <Header />
  <main>
    <Intro />
    <Benefits />
    <OurServices />
    <Gallery />
    <Testimonials />
    <ContactForm />
  </main>
  <Footer />
</template>

<style scoped>

</style>
