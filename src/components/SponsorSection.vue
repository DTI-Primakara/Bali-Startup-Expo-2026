<script setup lang="tsx">
import { motion } from 'motion-v'
</script>

<template>
  <section
    class="md:mb-40 md:pl-20 md:pr-20 pl-5 pr-5 flex flex-col items-center justify-center text-center relative"
  >
    <!-- shine decoration -->
    <div
      class="absolute w-150 h-150 rounded-full -top-30 -left-70 opacity-50 bg-[radial-gradient(circle,#022894,white)] blur-[200px] -z-100"
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
      <div class="star-1 rotate-75 w-20 h-20 -bottom-12 -right-17 absolute z-50"></div>

      <motion.h1
        :initial="{ y: 100, opacity: 0 }"
        :while-in-view="{ y: 0, opacity: 1 }"
        :transition="{ duration: 0.4 }"
        :in-view-options="{ once: true }"
        class="text-outline-2 md:text-6xl text-4xl font-bold"
        >Sponsor</motion.h1
      >
    </div>

    <motion.p
      :initial="{ y: 100, opacity: 0 }"
      :while-in-view="{ y: 0, opacity: 1 }"
      :transition="{ duration: 0.4 }"
      :in-view-options="{ once: true }"
      class="font-medium md:text-xl text-base"
    >
      Acara ini terselenggara berkat dukungan luar biasa dari para mitra dan sponsor resmi kami.
    </motion.p>

    <motion.div
      :initial="{ y: 100, opacity: 0 }"
      :while-in-view="{ y: 0, opacity: 1 }"
      :transition="{ duration: 0.4 }"
      :in-view-options="{ once: true }"
      class="w-full md:h-200 h-100 relative"
    >
      <!-- star decor -->
      <div class="star-1 rotate-92 w-20 h-20 top-17 left-78 absolute z-50"></div>
      <div class="star-1 rotate-78 w-20 h-20 bottom-35 md:-right-6 -right-12 absolute z-50"></div>

      <!-- rocket decor -->
      <div
        class="rocket rotate-90 md:w-45 md:h-45 w-20 h-20 bottom-10 md:-left-20 -left-7 absolute z-50"
      ></div>

      <!-- sponsor box -->
      <div class="sponsor-box absolute w-full md:h-200 h-80"></div>
    </motion.div>
  </section>
</template>
