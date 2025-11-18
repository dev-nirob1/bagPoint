<script setup>
import FooterSection from './components/sections/FooterSection.vue';
import NavbarSection from './components/sections/NavbarSection.vue';
import FormPopup from './components/widget/FormPopup.vue';
import VideoPopup from './components/widget/VideoPopup.vue';
import AboutUs from './zems/Front/Components/Section/AboutUs.vue';
import CtaSection from './zems/Front/Components/Section/CtaSection.vue';
import FeatureSection from './zems/Front/Components/Section/FeatureSection.vue';
import HeroSection from './zems/Front/Components/Section/HeroSection.vue';
import SpecificationSection from './zems/Front/Components/Section/SpecificationSection.vue';
import TestimonialSection from './zems/Front/Components/Section/TestimonialSection.vue';
import WhyChooseUs from './zems/Front/Components/Section/WhyChooseUs.vue';
import { ref } from 'vue'

const isVideoModalOpen = ref(false)
const isFormModalOpen = ref(false)

// video popup logic

const handleOpenVideoModal = () => {
  isVideoModalOpen.value = true
}
const handleCloseVideoModal = () => {
  isVideoModalOpen.value = false
}
// form popup logic

const handleOpenFormModal = () => {
  isFormModalOpen.value = true
}
const handleCloseFormModal = () => {
  isFormModalOpen.value = false
}

</script>

<template>
  <NavbarSection :handleOpenFormModal="handleOpenFormModal" />
  <HeroSection :handleOpenVideoModal="handleOpenVideoModal" :handleOpenFormModal="handleOpenFormModal" />
  <FeatureSection />
  <AboutUs :handleOpenVideoModal="handleOpenVideoModal" :handleOpenFormModal="handleOpenFormModal" />
  <WhyChooseUs />
  <SpecificationSection />
  <CtaSection :handleOpenFormModal="handleOpenFormModal" />
  <TestimonialSection />
  <FooterSection />
  <!-- video popup  -->
  <VideoPopup :isModalOpen="isVideoModalOpen" :handleCloseModal="handleCloseVideoModal" />
  <!-- form popup  -->
  <FormPopup :isFormModalOpen="isFormModalOpen" :handleCloseFormModal="handleCloseFormModal" />
</template>
