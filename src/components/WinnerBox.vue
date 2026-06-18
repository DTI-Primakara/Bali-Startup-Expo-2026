<script setup lang="tsx">
const props = defineProps({
  name: String,
  description: String,
  rank: String,
})
</script>

<template>
  <div :class="`winner-box-${rank} md:h-150 h-120 md:w-100 w-80 p-10 md:pt-107 pt-85`">
    <h2 class="font-extrabold md:text-3xl text-xl">{{ name }}</h2>
    <p class="font-medium md:text-base text-sm text-justify">{{ description }}</p>
  </div>
</template>
