<script setup lang="tsx">
import { motion } from 'motion-v'
</script>

<template>
  <section class="flex isolate relative mb-40 w-full items-center justify-center">
    <!-- wrapper -->
    <div class="grid grid-cols-[6fr_7fr] w-9/10 gap-10">
      <motion.div
        :initial="{ y: 100, opacity: 0 }"
        :while-in-view="{ y: 0, opacity: 1 }"
        :transition="{ duration: 0.4, delay: 0.4 }"
        :in-view-options="{ once: true }"
        class="w-full bg-red-400 h-100"
      ></motion.div>

      <motion.div
        :initial="{ y: 100, opacity: 0 }"
        :while-in-view="{ y: 0, opacity: 1 }"
        :transition="{ duration: 0.4 }"
        :in-view-options="{ once: true }"
        class="flex flex-col gap-4"
      >
        <p class="text-xl font-bold">About Us</p>
        <h1 class="text-outline-2 text-6xl font-bold">
          What is <br />
          Bali Start-Up Expo?
        </h1>

        <p class="text-gray text-xl font-medium">
          Bali Startup Expo adalah puncak inovasi technopreneur Primakara. Wadah kolaborasi yang
          menghubungkan puluhan startup digital pilihan dengan masyarakat dan dunia industri.
        </p>
      </motion.div>
    </div>
  </section>
</template>
