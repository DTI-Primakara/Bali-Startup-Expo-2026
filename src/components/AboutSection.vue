<script setup lang="tsx">
import { motion } from 'motion-v'
</script>

<template>
  <section
    id="about"
    class="scroll-m-35 flex isolate relative mb-20 w-full items-center justify-center"
  >
    <!-- star decor -->
    <div class="star-1 opacity-30 rotate-12 w-40 h-40 top-22 right-60 absolute -z-50"></div>
    <div class="star-1 opacity-60 rotate-22 w-15 h-15 bottom-0 right-60 absolute -z-50"></div>

    <!-- rocket decor -->
    <div class="rocket w-15 h-15 bottom-8 right-150 absolute -z-50"></div>

    <!-- moon decor -->
    <div class="moon w-20 h-20 -bottom-10 right-165 absolute -z-50"></div>

    <!-- wrapper -->
    <div class="md:grid grid-cols-[6fr_7fr] flex flex-col-reverse w-9/10 gap-10">
      <motion.div
        :initial="{ y: 100, opacity: 0 }"
        :while-in-view="{ y: 0, opacity: 1 }"
        :transition="{ duration: 0.4 }"
        :in-view-options="{ once: true }"
        class="w-full gap-6 grid grid-cols-2 grid-rows-2"
      >
        <div
          class="absolute w-40 h-40 rounded-full bg-[#031446] flex self-center justify-self-center items-center justify-center"
        >
          <div
            class="absolute w-27 h-27 rounded-full bg-linear-to-b bg-[#022894] to-[#0466C8] z-0"
          ></div>
          <p
            class="rounded-full w-24 h-24 font-bold text-xl justify-center items-center flex bg-[#031446] z-50"
          >
            BSE
          </p>
        </div>

        <img class="self-end justify-self-end" src="@/assets/images/about-1.png" />
        <img src="@/assets/images/about-2.png" />
        <img class="justify-self-end" src="@/assets/images/about-3.png" />
        <img src="@/assets/images/about-4.png" />
      </motion.div>

      <motion.div
        :initial="{ y: 100, opacity: 0 }"
        :while-in-view="{ y: 0, opacity: 1 }"
        :transition="{ duration: 0.4 }"
        :in-view-options="{ once: true }"
        class="flex flex-col gap-4 justify-center md:items-start md:text-left text-center items-center"
      >
        <p class="text-xl font-bold">About Us</p>
        <h1 class="text-outline-2 md:text-6xl text-4xl font-bold">
          What is <br />
          Bali Start-Up Expo?
        </h1>

        <p class="text-gray md:text-xl text-base font-medium">
          Bali Startup Expo adalah puncak inovasi technopreneur Primakara. Wadah kolaborasi yang
          menghubungkan puluhan startup digital pilihan dengan masyarakat dan dunia industri.
        </p>
      </motion.div>
    </div>
  </section>
</template>
