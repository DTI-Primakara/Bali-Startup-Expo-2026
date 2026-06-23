<script setup lang="tsx">
import { motion } from 'motion-v'
const props = defineProps({
  title: String,
  description: String,
  topic: String,
  time: String,
  speaker: String,
})
</script>

<template>
  <motion.div
    :initial="{ y: 100, opacity: 0 }"
    :while-in-view="{ y: 0, opacity: 1 }"
    :transition="{ duration: 0.4 }"
    :in-view-options="{ once: true }"
    class="w-full h-full gap-2 backdrop-blur-sm rounded-[10px] md:p-10 p-7 pb-5 flex flex-col md:items-start items-center justify-center bg-white/15 shadow-[0_0_4px_2px_rgba(255,255,255,0.4)]"
  >
    <p
      class="font-semibold md:text-2xl text-base absolute md:block hidden top-4 right-4 underline underline-offset-8"
    >
      Free Entry
    </p>
    <h2 class="md:text-3xl text-2xl font-semibold text-center md:text-left">{{ title }}</h2>
    <p class="md:text-xl text-base mb-4 font-medium text-gray text-center md:text-left">
      {{ description }}
    </p>

    <div class="mb-3 md:text-xl text-base font-medium grid gap-3 grid-cols-[1fr_10fr] items-center">
      <img src="../assets/images/icon-document.png" />
      <p>: {{ topic }}</p>

      <img src="../assets/images/icon-time.png" />
      <p>: {{ time }}</p>

      <img src="../assets/images/icon-microphone.png" />
      <p>: {{ speaker }}</p>
    </div>

    <a href="test" class="font-semibold text-base underline underline-offset-5"
      >Book your seat now</a
    >
  </motion.div>
</template>
