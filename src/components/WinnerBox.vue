<script setup lang="tsx">
const props = defineProps({
  name: String,
  description: String,
  rank: String,
})
</script>

<template>
  <div :class="`winner-box-${rank} h-150 w-100 p-8 pt-107`">
    <h2 class="font-extrabold text-3xl">{{ name }}</h2>
    <p class="font-medium text-base text-justify">{{ description }}</p>
  </div>
</template>
