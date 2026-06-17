<script setup lang="ts">
import AboutSection from './components/AboutSection.vue'
import ActivitySection from './components/ActivitySection.vue'
import Footer from './components/Footer.vue'
import GallerySection from './components/GallerySection.vue'
import Header from './components/Header.vue'
import HeroSection from './components/HeroSection.vue'
import HistorySection from './components/HistorySection.vue'
import InvitationSection from './components/InvitationSection.vue'
import MediaPartnerSection from './components/MediaPartnerSection.vue'
import SideEventSection from './components/SideEventSection.vue'
import SponsorSection from './components/SponsorSection.vue'
import WinnerSection from './components/WinnerSection.vue'
</script>

<template>
  <Header />

  <HeroSection />
  <AboutSection />
  <HistorySection />
  <ActivitySection />
  <SideEventSection />
  <WinnerSection />
  <SponsorSection />
  <MediaPartnerSection />
  <GallerySection />
  <InvitationSection />

  <Footer />
</template>
