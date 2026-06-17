<script setup lang="tsx">
const props = defineProps({
  title: String,
  description: String,
  topic: String,
  time: String,
  speaker: String,
})
</script>

<template>
  <div
    class="w-full h-full gap-2 backdrop-blur-sm rounded-[10px] p-10 pb-5 flex flex-col justify-center bg-white/15 shadow-[0_0_4px_2px_rgba(255,255,255,0.4)]"
  >
    <p class="font-semibold text-2xl absolute top-4 right-4 underline underline-offset-8">
      Free Entry
    </p>
    <h2 class="text-3xl font-semibold">{{ title }}</h2>
    <p class="text-xl mb-4 font-medium text-gray">{{ description }}</p>

    <div class="mb-3 text-xl font-medium grid gap-2 grid-cols-[1fr_10fr] grid-rows-2 items-center">
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
  </div>
</template>
