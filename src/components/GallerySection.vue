<script setup lang="tsx">
import { motion } from 'motion-v'
</script>

<template>
  <section
    id="gallery"
    class="scroll-m-45 mb-40 md:pl-20 md:pr-20 pl-5 pr-5 flex flex-col items-center justify-center text-center relative"
  >
    <!-- shine decoration -->
    <div
      class="absolute w-150 h-150 rounded-full top-110 -left-70 opacity-50 bg-[radial-gradient(circle,#022894,white)] blur-[200px] -z-100"
    ></div>
    <div
      class="absolute w-150 h-150 rounded-full top-70 -right-70 opacity-50 bg-[radial-gradient(circle,#022894,white)] blur-[200px] -z-100"
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
        >Gallery</motion.h1
      >
    </div>

    <motion.p
      :initial="{ y: 100, opacity: 0 }"
      :while-in-view="{ y: 0, opacity: 1 }"
      :transition="{ duration: 0.4 }"
      :in-view-options="{ once: true }"
      class="mb-12 font-medium md:text-xl text-base"
    >
      Intip kembali keseruan, antusiasme, dan momen-momen inspiratif yang terekam sepanjang gelaran
      Bali Startup Expo.
    </motion.p>

    <div class="grid grid-cols-21 gap-2">
      <!-- first row -->
      <img class="col-span-6 h-full w-full object-cover" src="/images/gallery-1.png" />
      <img class="col-span-5 h-full w-full object-cover" src="/images/gallery-2.png" />
      <img class="col-span-10 h-full w-full object-cover" src="/images/gallery-3.png" />

      <!-- second row -->
      <img class="col-span-8 h-full w-full object-cover" src="/images/gallery-4.png" />
      <img class="col-span-7 h-full w-full object-cover" src="/images/gallery-5.png" />
      <img class="col-span-6 h-full w-full object-cover" src="/images/gallery-6.png" />

      <!-- third row -->
      <img class="col-span-5 h-full w-full object-cover" src="/images/gallery-7.png" />
      <img class="col-span-6 h-full w-full object-cover" src="/images/gallery-8.png" />
      <img class="col-span-5 h-full w-full object-cover" src="/images/gallery-9.png" />
      <img class="col-span-5 h-full w-full object-cover" src="/images/gallery-10.png" />
    </div>
  </section>
</template>
