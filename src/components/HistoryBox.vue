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
    class="self-end relative mb-20 w-190 h-120 pr-10 pl-15 pt-27 gap-4 items-end flex flex-col text-justify"
    v-if="mirrored"
  >
    <!-- box shape -->
    <div class="history-box w-full h-full absolute left-0 top-0 -scale-x-100 -z-50"></div>

    <h2 class="font-semibold text-5xl">{{ year }}</h2>
    <h3 class="font-semibold text-4xl">{{ title }}</h3>
    <p class="font-medium text-2xl">{{ description }}</p>
  </motion.div>

  <motion.div
    :initial="{ y: 100, opacity: 0 }"
    :while-in-view="{ y: 0, opacity: 1 }"
    :transition="{ duration: 0.4 }"
    :in-view-options="{ once: true }"
    class="history-box mb-20 w-190 h-120 pl-10 pr-15 pt-27 gap-4 flex flex-col text-justify self-start"
    v-if="!mirrored"
  >
    <h2 class="font-semibold text-5xl">{{ year }}</h2>
    <h3 class="font-semibold text-4xl">{{ title }}</h3>
    <p class="font-medium text-2xl">{{ description }}</p>
  </motion.div>
</template>
