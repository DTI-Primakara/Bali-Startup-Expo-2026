<script setup lang="tsx">
import { motion } from 'motion-v'

const props = defineProps({
  index: Number,
  currentIndex: Number,
  comingSoon: Boolean,
})
</script>

<template>
  <motion.div
    :initial="{ y: 100, opacity: 0 }"
    :while-in-view="{ y: 0, opacity: 1 }"
    :transition="{ duration: 0.4 }"
    :in-view-options="{ once: true }"
    class="w-full gap-2 backdrop-blur-sm rounded-[10px] md:p-10 p-7 flex flex-col justify-center bg-white/15 shadow-[0_0_4px_2px_rgba(255,255,255,0.4)] duration-500"
    :style="{
      filter: currentIndex != index ? `brightness(80%)` : '',
      transform: currentIndex != index ? `translateY(24px)` : '',
    }"
  >
    <div
      v-if="comingSoon"
      class="flex flex-col items-center justify-center h-100 relative text-center"
    >
      <!-- rocket decor -->
      <div class="rocket rotate-135 w-25 h-25 bottom-8 absolute -z-50"></div>

      <div class="relative">
        <!-- star decor -->
        <div class="star-1 -rotate-112 w-40 h-40 -top-16 -right-22 absolute z-50"></div>
        <h2 class="text-[#FEFCFB] font-bold italic md:text-8xl text-5xl text-outline-1">
          COMING SOON
        </h2>
      </div>

      <h3 class="text-[#FEFCFB] font-bold italic md:text-5xl text-2xl text-outline-1">
        -- Stay Tuned --
      </h3>
    </div>

    <div v-if="!comingSoon" class="gap-10 md:grid grid-cols-2 flex flex-col">
      <div class="w-full md:h-90 h-40 bg-red-500"></div>
      <div class="w-full flex flex-col justify-center md:items-start items-center">
        <div class="mb-4 relative">
          <!-- border decoration -->
          <div
            class="h-6 w-20 border-white border-l-2 border-t-2 absolute -top-0.5 -left-3 rounded-tl-sm blur-md"
          ></div>
          <div
            class="h-6 w-20 border-white border-l-2 border-t-2 absolute -top-0.5 -left-3 rounded-tl-sm"
          ></div>

          <div
            class="h-6 w-20 border-white border-r-2 border-b-2 absolute -bottom-0.5 -right-3 rounded-br-sm blur-md"
          ></div>
          <div
            class="h-6 w-20 border-white border-r-2 border-b-2 absolute -bottom-0.5 -right-3 rounded-br-sm"
          ></div>

          <h2 class="text-outline-2 md:text-3xl text-xl font-bold">Special Perform</h2>
        </div>

        <p class="mb-8 font-medium md:text-xl text-base md:text-left text-center">
          Figma ipsum component variant main layer. Inspect clip opacity effect style invite export.
          Polygon pixel team layout hand inspect team.
        </p>

        <div class="grid-cols-[1fr_auto] gap-y-2 gap-x-2 grid items-center">
          <img src="../assets/images/icon-calender.png" />
          <p class="text-base font-medium">10 Juli 2026</p>

          <img src="../assets/images/icon-time.png" />
          <p class="text-base font-medium">10:00-11:00 WITA</p>

          <img src="../assets/images/icon-location.png" />
          <p class="text-base font-medium">Discovery Mall</p>
        </div>
      </div>
    </div>
  </motion.div>
</template>
