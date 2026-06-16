<script setup lang="tsx">
import { motion } from 'motion-v'
</script>

<template>
  <section
    class="h-[130vh] w-full gap-4 pt-40 mb-15 items-center justify-center flex flex-col text-center relative isolate overflow-hidden"
  >
    <!-- shine decoration -->
    <div
      class="absolute w-150 h-150 rounded-full -left-100 -top-100 opacity-50 bg-[radial-gradient(circle,#022894,white)] blur-[200px] -z-50"
    ></div>
    <div
      class="absolute w-150 h-150 rounded-full -right-75 -top-75 opacity-50 bg-[radial-gradient(circle,#022894,white)] blur-[200px] -z-50"
    ></div>

    <div class="relative">
      <!-- border decoration -->
      <div
        class="h-6 w-20 border-white border-l-2 border-t-2 absolute top-0 -left-1.5 rounded-tl-sm blur-md"
      ></div>
      <div
        class="h-6 w-20 border-white border-l-2 border-t-2 absolute top-0 -left-1.5 rounded-tl-sm"
      ></div>

      <div
        class="h-6 w-20 border-white border-r-2 border-b-2 absolute bottom-0 -right-1.5 rounded-br-sm blur-md"
      ></div>
      <div
        class="h-6 w-20 border-white border-r-2 border-b-2 absolute bottom-0 -right-1.5 rounded-br-sm"
      ></div>

      <h2 class="text-4xl font-semibold">Ignite the Courage, Empower the Future</h2>
    </div>

    <div class="relative flex items-center justify-center">
      <!-- shine decoration -->
      <div
        class="absolute w-25 h-25 rounded-full -bottom-70 mr-70 opacity-50 bg-[radial-gradient(circle,#022894,white)] blur-[25px] -z-50"
      ></div>

      <!-- star decoration -->
      <div class="star -rotate-6 w-45 h-45 -top-35 -left-15 absolute z-50"></div>
      <div class="star rotate-6 w-20 h-20 -top-15 right-0 absolute z-50"></div>

      <!-- rocket decoration -->
      <div class="rocket w-25 h-25 rotate-90 -bottom-20 -left-30 absolute z-50"></div>
      <div class="rocket w-45 h-45 -bottom-65 -right-40 absolute z-50"></div>

      <motion.h1
        :initial="{ y: 100, opacity: 0 }"
        :while-in-view="{ y: 0, opacity: 1 }"
        :transition="{ duration: 0.4 }"
        :in-view-options="{ once: true }"
        class="text-[#FEFCFB] font-bold text-8xl text-outline-1"
      >
        Bali Start-Up Expo
      </motion.h1>
    </div>

    <h3 class="font-medium text-xl max-w-7/10">
      Panggung inovasi terbesar bagi startup lokal Bali. Temukan ide brilian, bangun koneksi
      strategis, dan jadilah bagian dari revolusi ekonomi digital masa depan.
    </h3>

    <!-- <button class="cursor-pointer border-2 border-white p-4 pt-2 pb-2 relative shadow-[0_0_16px_1px_rgba(255,255,255,0.3),inset_0_0_16px_1px_rgba(255,255,255,0.3)]"> -->
    <!-- decorations -->
    <!-- <div class="star rotate-90 w-10 h-10 -bottom-5 -left-5 absolute z-50"></div> -->
    <!-- <div class="star rotate-90 w-10 h-10 -top-5 -right-5 absolute z-50"></div> -->

    <!-- <div class="absolute w-full h-full border border-white top-0 left-0 blur-sm"></div> -->
    <!-- <p class="">Lihat Selengkapnya</p> -->
    <!-- </button> -->

    <button class="mb-8 p-3 border-white border rounded-4xl">
      <p class="text-lg font-semibold">📍Discovery Mall Bali</p>
    </button>

    <!-- title & motto
    <div class="h-full w-full items-center justify-center flex flex-col text-center justify-self-center gap-4">

    </div> -->

    <div
      class="w-7/10 backdrop-blur-sm rounded-[10px] p-10 flex justify-between bg-white/2 shadow-[0_0_1px_1px_rgba(255,255,255,0.35),0_0_1px_1px_rgba(0,0,0,1)]"
    >
      <div class="w-1/4 bg-[radial-gradient(circle,rgba(4,102,200,0.5),transparent,transparent)]">
        <p class="text-6xl medium">00</p>
        <p class="text-3xl medium">Days</p>
      </div>
      <div class="w-1/4 bg-[radial-gradient(circle,rgba(4,102,200,0.5),transparent,transparent)]">
        <p class="text-6xl medium">00</p>
        <p class="text-3xl medium">Hours</p>
      </div>
      <div class="w-1/4 bg-[radial-gradient(circle,rgba(4,102,200,0.5),transparent,transparent)]">
        <p class="text-6xl medium">00</p>
        <p class="text-3xl medium">Minutes</p>
      </div>
      <div class="w-1/4 bg-[radial-gradient(circle,rgba(4,102,200,0.5),transparent,transparent)]">
        <p class="text-6xl medium">00</p>
        <p class="text-3xl medium">Seconds</p>
      </div>
    </div>
  </section>
</template>
