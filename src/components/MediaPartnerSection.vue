<script setup lang="ts">
import { motion } from 'motion-v'
import MediaPartnerBox from './MediaPartnerBox.vue'

const MEDIA_PARTNER_COUNT = 15
</script>

<template>
  <section class="w-full mb-35 pt-10 flex flex-col items-center text-center relative">
    <!-- shine decoration -->
    <div
      class="absolute w-150 h-150 rounded-full -top-10 -right-100 opacity-50 bg-[radial-gradient(circle,#022894,white)] blur-[200px] -z-100"
    ></div>

    <div class="mb-7 relative">
      <!-- border decoration -->
      <div
        class="h-6 w-20 border-white border-l-2 border-t-2 absolute -top-2 -left-7.5 rounded-tl-sm blur-md"
      ></div>
      <div
        class="h-6 w-20 border-white border-l-2 border-t-2 absolute -top-2 -left-7.5 rounded-tl-sm"
      ></div>

      <div
        class="h-6 w-20 border-white border-r-2 border-b-2 absolute -bottom-2 -right-7.5 rounded-br-sm blur-md"
      ></div>
      <div
        class="h-6 w-20 border-white border-r-2 border-b-2 absolute -bottom-2 -right-7.5 rounded-br-sm"
      ></div>

      <!-- star decor -->
      <div class="star-1 rotate-75 w-30 h-30 -top-17 -left-22 absolute z-50"></div>

      <motion.h1
        :initial="{ y: 100, opacity: 0 }"
        :while-in-view="{ y: 0, opacity: 1 }"
        :transition="{ duration: 0.4 }"
        :in-view-options="{ once: true }"
        class="text-outline-2 md:text-6xl text-4xl font-bold"
        >Media Partner</motion.h1
      >
    </div>

    <motion.p
      :initial="{ y: 100, opacity: 0 }"
      :while-in-view="{ y: 0, opacity: 1 }"
      :transition="{ duration: 0.4 }"
      :in-view-options="{ once: true }"
      class="mb-10 md:text-xl md:pl-20 md:pr-20 pl-10 pr-10 text-base font-medium"
    >
      Figma ipsum component variant main layer. Inspect clip opacity effect style invite export.
      Polygon pixel team layout hand inspect team.
    </motion.p>

    <div class="w-full overflow-hidden">
      <div class="w-max flex self-start infinite-marquee">
        <MediaPartnerBox
          v-for="index in MEDIA_PARTNER_COUNT"
          :key="`media_partner_${index}`"
          :index="index"
        />

        <MediaPartnerBox
          v-for="index in MEDIA_PARTNER_COUNT"
          :key="`media_partner_${index}`"
          :index="index"
        />
      </div>
    </div>
  </section>
</template>

<style lang="css" scoped>
@keyframes infinite-marquee-animation {
  0% {
    transform: translateX(0);
  }

  100% {
    transform: translateX(-50%);
  }
}

.infinite-marquee {
  animation: infinite-marquee-animation 30s linear infinite;
}
</style>
