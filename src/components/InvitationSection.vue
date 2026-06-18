<script setup lang="tsx">
import { motion } from 'motion-v'
</script>

<template>
  <section
    class="h-screen md:pl-20 md:pr-20 pl-10 pr-10 gap-6 flex flex-col items-center justify-center text-center relative"
  >
    <!-- gradient circle -->
    <div
      class="absolute w-100 h-100 md:mb-100 mb-0 rounded-full opacity-50 bg-[radial-gradient(circle,#007FFF,#007FFF)] blur-[150px] -z-100"
    ></div>

    <!-- star decor -->
    <div class="star-1 rotate-45 opacity-20 w-30 h-30 top-0 left-20 absolute -z-50"></div>
    <div class="star-1 rotate-45 opacity-20 w-30 h-30 top-10 left-60 absolute -z-50"></div>
    <div class="star-1 rotate-45 opacity-20 w-30 h-30 -top-10 left-120 absolute -z-50"></div>
    <div class="star-1 rotate-45 opacity-20 w-30 h-30 top-80 left-20 absolute -z-50"></div>
    <div class="star-1 rotate-45 opacity-20 w-20 h-20 top-80 left-60 absolute -z-50"></div>
    <div class="star-1 -rotate-11 w-20 h-20 top-50 left-50 absolute -z-50"></div>

    <div class="star-1 rotate-45 opacity-20 w-30 h-30 -top-10 right-120 absolute -z-50"></div>
    <div class="star-1 rotate-45 opacity-20 w-30 h-30 top-20 right-60 absolute -z-50"></div>
    <div class="star-1 rotate-45 opacity-20 w-30 h-30 top-30 right-20 absolute -z-50"></div>
    <div class="star-1 rotate-45 opacity-20 w-30 h-30 top-70 right-20 absolute -z-50"></div>
    <div class="star-1 rotate-45 opacity-20 w-30 h-30 top-80 right-50 absolute -z-50"></div>
    <div class="star-1 -rotate-11 w-20 h-20 top-55 right-50 absolute -z-50"></div>

    <p class="font-semibold text-sm text-[#164CA4]">FINAL COUNTDOWN</p>
    <motion.p
      :initial="{ y: 100, opacity: 0 }"
      :while-in-view="{ y: 0, opacity: 1 }"
      :transition="{ duration: 0.4 }"
      :in-view-options="{ once: true }"
      class="font-semibold md:text-5xl text-3xl"
    >
      Ready To Launch <br />
      Your Future?
    </motion.p>
    <motion.p
      :initial="{ y: 100, opacity: 0 }"
      :while-in-view="{ y: 0, opacity: 1 }"
      :transition="{ duration: 0.4 }"
      :in-view-options="{ once: true }"
      class="mb-8 font-medium md:text-base text-sm text-gray"
    >
      Join Bali Startup Expo 2026 and Become Part of Bali’s Innovation
    </motion.p>

    <button
      class="rounded-[50px] p-8 pl-12 pr-12 font-semibold text-xl bg-linear-to-r bg-[#0466C8] to-[#033E79] flex items-center gap-4 cursor-pointer"
    >
      Register Now
      <img class="h-5 w-5" src="../assets/images/right-arrow.png" />
    </button>
  </section>
</template>
