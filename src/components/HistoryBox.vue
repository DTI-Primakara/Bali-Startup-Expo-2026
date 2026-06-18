<script setup lang="tsx">
import { motion } from 'motion-v'

const props = defineProps({
  mirrored: Boolean,
  year: String,
  title: String,
  description: String,
})
</script>

<template>
  <motion.div
    :initial="{ y: 100, opacity: 0 }"
    :while-in-view="{ y: 0, opacity: 1 }"
    :transition="{ duration: 0.4 }"
    :in-view-options="{ once: true }"
    class="self-end relative mb-20 md:w-190 w-full md:h-120 p-10 md:pr-10 md:pl-15 md:pt-27 gap-4 md:items-end items-center flex flex-col md:backdrop-blur-none backdrop-blur-sm md:rounded-none rounded-[10px] md:bg-transparent bg-white/15 md:shadow-none shadow-[0_0_4px_2px_rgba(255,255,255,0.4)]"
    v-if="mirrored"
  >
    <!-- box shape -->
    <div
      class="history-box w-full h-full absolute left-0 top-0 -scale-x-100 -z-50 md:block hidden"
    ></div>

    <h2 class="font-semibold md:text-5xl text-3xl md:text-right">{{ year }}</h2>
    <h3 class="font-semibold md:text-4xl text-2xl md:text-right">{{ title }}</h3>
    <p class="font-medium md:text-2xl text-base md:text-justify">{{ description }}</p>
  </motion.div>

  <motion.div
    :initial="{ y: 100, opacity: 0 }"
    :while-in-view="{ y: 0, opacity: 1 }"
    :transition="{ duration: 0.4 }"
    :in-view-options="{ once: true }"
    class="relative mb-20 md:w-190 w-full md:h-120 p-10 md:pl-10 md:pr-15 md:pt-27 gap-4 flex md:items-start flex-col self-start md:backdrop-blur-none backdrop-blur-sm md:rounded-none rounded-[10px] md:bg-transparent bg-white/15 md:shadow-none shadow-[0_0_4px_2px_rgba(255,255,255,0.4)]"
    v-if="!mirrored"
  >
    <!-- box shape -->
    <div class="history-box w-full h-full absolute left-0 top-0 -z-50 md:block hidden"></div>

    <h2 class="font-semibold md:text-5xl text-3xl md:text-left">{{ year }}</h2>
    <h3 class="font-semibold md:text-4xl text-2xl md:text-left">{{ title }}</h3>
    <p class="font-medium md:text-2xl text-base md:text-justify">{{ description }}</p>
  </motion.div>
</template>
