<script setup lang="ts">
import { motion } from 'motion-v'
import WinnerBox from './WinnerBox.vue'
</script>

<template>
  <section
    class="mb-50 md:pl-20 md:pr-20 pl-10 pr-10 flex flex-col items-center justify-center text-center relative"
  >
    <!-- shine decoration -->
    <div
      class="absolute w-150 h-150 rounded-full -top-50 -right-70 opacity-50 bg-[radial-gradient(circle,#022894,white)] blur-[200px] -z-100"
    ></div>

    <!-- rocket decor -->
    <div class="rocket rotate-90 w-45 h-45 -top-40 left-0 absolute -z-50"></div>
    <div class="rocket w-45 h-45 -bottom-55 right-20 absolute -z-50"></div>

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
        class="text-outline-2 md:text-6xl text-4xl font-bold md:w-fit w-min"
        >Winner of 2025</motion.h1
      >
    </div>

    <motion.p
      :initial="{ y: 100, opacity: 0 }"
      :while-in-view="{ y: 0, opacity: 1 }"
      :transition="{ duration: 0.4 }"
      :in-view-options="{ once: true }"
      class="mb-15 md:text-xl text-base font-medium"
    >
      Rayakan inovasi tanpa batas. Inilah deretan startup terbaik yang berhasil menginspirasi dan
      memberikan solusi nyata di Bali Startup Expo 2025.
    </motion.p>

    <motion.div
      :initial="{ y: 100, opacity: 0 }"
      :while-in-view="{ y: 0, opacity: 1 }"
      :transition="{ duration: 0.4 }"
      :in-view-options="{ once: true }"
      class="w-full md:gap-0 gap-8 flex md:flex-row flex-col items-center justify-center"
    >
      <!-- different order on phone -->
      <div class="relative flex justify-center md:hidden">
        <!-- star decor -->
        <div class="star-1 rotate-78 w-20 h-20 -top-7 ml-10 absolute z-50"></div>
        <div class="star-1 rotate-78 w-20 h-20 top-0 -right-3 absolute z-50"></div>
        <div class="star-1 rotate-78 w-20 h-20 -bottom-10 -left-8 absolute z-50"></div>

        <WinnerBox
          rank="1"
          name="Pesona Plastik"
          description="Inovasi dekorasi interior yang memadukan estetika seni rupa dengan teknologi pencahayaan modern yang memukau."
        />
      </div>

      <div class="relative">
        <!-- star decor -->
        <div class="star-1 rotate-4 w-20 h-20 top-0 -right-5 absolute z-50"></div>

        <WinnerBox
          rank="2"
          name="Lightbox Painting"
          description="Transformasi kreatif limbah plastik menjadi produk bernilai guna tinggi melalui inovasi ekonomi sirkular yang berkelanjutan."
        />
      </div>

      <div class="relative hidden justify-center md:flex">
        <!-- star decor -->
        <div class="star-1 rotate-78 w-20 h-20 -top-7 ml-10 absolute z-50"></div>
        <div class="star-1 rotate-78 w-20 h-20 top-0 -right-3 absolute z-50"></div>
        <div class="star-1 rotate-78 w-20 h-20 -bottom-10 -left-8 absolute z-50"></div>

        <WinnerBox
          rank="1"
          name="Pesona Plastik"
          description="Inovasi dekorasi interior yang memadukan estetika seni rupa dengan teknologi pencahayaan modern yang memukau."
        />
      </div>

      <div>
        <WinnerBox
          rank="3"
          name="Green Oil Solution"
          description="Solusi cerdas pengelolaan minyak jelantah untuk menekan polusi sekaligus menciptakan sumber energi terbarukan."
        />
      </div>
    </motion.div>
  </section>
</template>
