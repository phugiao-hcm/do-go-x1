<template>
  <div>
    <HeroSectionSlide />
    <HeroSection />
    <ServiceSection />

    <FeaturedSlider />
    <CustomerFeedback />
    <NewsSection />
  </div>
</template>

<script setup>
import HeroSectionSlide from "../components/home/HeroSectionSlide.vue";
import HeroSection from "../components/home/HeroSection.vue";
import FeaturedSlider from "../components/home/FeaturedSlider.vue";
import ServiceSection from "../components/home/ServiceSection.vue";
import CustomerFeedback from "../components/home/CustomerFeedback.vue";
import NewsSection from "../components/home/NewsSection.vue";
</script>
