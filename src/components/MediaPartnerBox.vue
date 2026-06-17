<script setup lang="tsx">
const props = defineProps({
  index: Number,
})
</script>

<template>
  <div class="media-partner-box shrink-0 w-80 h-60 relative flex items-center justify-center pb-4">
    <!-- star decor -->
    <div class="star-1 -rotate-6 w-20 h-20 -top-6 -left-6 absolute z-50"></div>
    <div class="star-1 -rotate-6 w-20 h-20 bottom-2 right-0 absolute z-50"></div>

    <img class="h-30 w-30" :src="`/media-partner/media-partner-${index}.png`" />
  </div>
</template>
