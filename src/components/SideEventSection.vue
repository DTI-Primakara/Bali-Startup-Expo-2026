<script setup lang="tsx">
import { motion } from 'motion-v'
import SideEventBox from './SideEventBox.vue'
import { ref } from 'vue'

const CAROUSEL_COUNT = 3
const carouselIndex = ref(0)

const handleCarousel = (direction: 'left' | 'right') => {
  if (direction == 'left') {
    carouselIndex.value = (carouselIndex.value - 1) % CAROUSEL_COUNT

    if (carouselIndex.value < 0) {
      carouselIndex.value = CAROUSEL_COUNT - 1
    }
  } else if (direction == 'right') {
    carouselIndex.value = (carouselIndex.value + 1) % CAROUSEL_COUNT
  }
}
</script>

<template>
  <section
    id="side-event"
    class="scroll-m-45 mb-50 md:pl-20 md:pr-20 pl-5 pr-5 flex flex-col items-center relative"
  >
    <!-- shine decoration -->
    <div
      class="absolute w-150 h-150 rounded-full -top-20 -left-70 opacity-50 bg-[radial-gradient(circle,#022894,white)] blur-[200px] -z-100"
    ></div>

    <div class="mb-25 relative">
      <!-- border decoration -->
      <div
        class="h-6 w-20 border-white border-l-2 border-t-2 absolute -top-2 -left-7.5 rounded-tl-sm blur-md"
      ></div>
      <div
        class="h-6 w-20 border-white border-l-2 border-t-2 absolute -top-2 -left-7.5 rounded-tl-sm"
      ></div>

      <div
        class="h-6 w-20 border-white border-r-2 border-b-2 absolute -bottom-2 -right-7.5 rounded-br-sm blur-md"
      ></div>
      <div
        class="h-6 w-20 border-white border-r-2 border-b-2 absolute -bottom-2 -right-7.5 rounded-br-sm"
      ></div>

      <!-- star decor -->
      <div class="star-1 rotate-75 w-30 h-30 -bottom-17 -right-22 absolute z-50"></div>

      <motion.h1
        :initial="{ y: 100, opacity: 0 }"
        :while-in-view="{ y: 0, opacity: 1 }"
        :transition="{ duration: 0.4 }"
        :in-view-options="{ once: true }"
        class="text-outline-2 md:text-6xl text-4xl font-bold text-center md:w-fit w-min"
        >Special Perform</motion.h1
      >
    </div>

    <div class="flex w-[300%] self-start items-center">
      <div
        class="grid grid-cols-3 pl-4 pr-4 items-center justify-center self-start w-full gap-8 relative duration-750"
        :style="{ transform: `translateX(-${(carouselIndex / 3) * 100}%)` }"
      >
        <side-event-box
          v-for="index in CAROUSEL_COUNT"
          :index="index - 1"
          :current-index="carouselIndex"
          :coming-soon="true"
        />
      </div>
    </div>

    <div class="mt-6 flex gap-2 relative items-center">
      <button
        v-on:click="handleCarousel('left')"
        class="text-xl font-bold absolute h-10 w-10 rounded-full -left-14 z-50 bg-white/30 shadow-[inset_0_0_6px_1px_rgba(255,255,255,0.4)] backdrop-blur-sm cursor-pointer"
      >
        <
      </button>
      <button
        v-on:click="handleCarousel('right')"
        class="text-xl font-bold absolute h-10 w-10 rounded-full -right-14 z-50 bg-white/30 shadow-[inset_0_0_6px_1px_rgba(255,255,255,0.4)] backdrop-blur-sm cursor-pointer"
      >
        >
      </button>

      <div
        v-for="index in CAROUSEL_COUNT"
        class="h-5 w-5 rounded-full bg-white/30 shadow-[inset_0_0_4px_2px_rgba(255,255,255,0.4)] backdrop-blur-sm brightness-80"
      ></div>

      <!-- formula: (width+gap) * index -->
      <div
        class="translate-x-${(5 + 2) * carouselIndex} h-5 w-5 rounded-full bg-white/30 shadow-[inset_0_0_4px_2px_rgba(255,255,255,0.4)] backdrop-blur-sm absolute duration-750"
        :style="{ transform: `translateX(${(5 + 2) * carouselIndex * 4}px)` }"
      ></div>
    </div>
  </section>
</template>
