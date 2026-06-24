<script setup lang="tsx">
import { ref } from 'vue'

const EVENT_DATE = new Date('2026-07-09T00:00:00')

const formatNumber = (value: number): string => {
  if (value < 10) {
    return `0${value}`
  } else {
    return value.toString()
  }
}

const secondsRef = ref('00')
const minutesRef = ref('00')
const hoursRef = ref('00')
const daysRef = ref('00')

const updateDateDiff = () => {
  let seconds = Math.round((EVENT_DATE.getTime() - new Date().getTime()) / 1000),
    minutes = 0,
    hours = 0,
    days = 0

  if (seconds < 0) {
    return
  }

  if (seconds >= 60) {
    minutes = Math.floor(seconds / 60)
    seconds -= minutes * 60
  }

  if (minutes >= 60) {
    hours = Math.floor(minutes / 60)
    minutes -= hours * 60
  }

  if (hours >= 24) {
    days = Math.floor(hours / 24)
    hours -= days * 24
  }

  secondsRef.value = formatNumber(seconds)
  minutesRef.value = formatNumber(minutes)
  hoursRef.value = formatNumber(hours)
  daysRef.value = formatNumber(days)
}

updateDateDiff()

// countdown
setInterval(() => {
  updateDateDiff()
}, 1 * 1000)
</script>

<template>
  <section
    id="hero"
    class="w-full gap-4 pl-10 pr-10 md:pl-20 md:pr-20 md:pt-50 pt-40 mb-40 items-center justify-center flex flex-col text-center relative isolate"
  >
    <!-- star decor -->
    <div class="star-2 opacity-60 bottom-0 left-10 absolute w-45 h-45 -z-50"></div>

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

      <!-- star decoration -->
      <div class="star-1 rotate-15 w-45 h-45 -top-22 -left-32 absolute -z-50"></div>
      <div class="star-1 opacity-60 rotate-6 w-20 h-20 -bottom-12 -right-18 absolute -z-50"></div>

      <h2 class="md:text-4xl text-2xl font-semibold">Ignite the Courage, Empower the Future</h2>
    </div>

    <div class="relative flex items-center justify-center">
      <!-- shine decoration -->
      <div
        class="absolute w-25 h-25 rounded-full -bottom-70 mr-70 opacity-50 bg-[radial-gradient(circle,#022894,white)] blur-[25px] -z-50"
      ></div>

      <!-- rocket decoration -->
      <div class="rocket w-25 h-25 rotate-90 -bottom-10 -left-30 absolute -z-50"></div>
      <div class="rocket w-45 h-45 -bottom-65 -right-40 absolute -z-50"></div>

      <h1 class="text-[#FEFCFB] font-bold md:text-8xl text-6xl text-outline-1">
        Bali Start-Up Expo
      </h1>
    </div>

    <h3 class="font-medium md:text-xl text-base">
      Panggung inovasi terbesar bagi startup lokal Bali. Temukan ide brilian, bangun koneksi
      strategis, dan jadilah bagian dari revolusi ekonomi digital masa depan.
    </h3>

    <!-- <button class="cursor-pointer border-2 border-white p-4 pt-2 pb-2 relative shadow-[0_0_16px_1px_rgba(255,255,255,0.3),inset_0_0_16px_1px_rgba(255,255,255,0.3)]"> -->
    <!-- decorations -->
    <!-- <div class=" rotate-90 w-10 h-10 -bottom-5 -left-5 absolute z-50"></div> -->
    <!-- <div class="star rotate-90 w-10 h-10 -top-5 -right-5 absolute z-50"></div> -->

    <!-- <div class="absolute w-full h-full border border-white top-0 left-0 blur-sm"></div> -->
    <!-- <p class="">Lihat Selengkapnya</p> -->
    <!-- </button> -->

    <a
      href="https://maps.app.goo.gl/QFua9m7JCx8yQpxYA"
      target="_blank"
      class="mb-8 p-3 border-white border rounded-4xl duration-200 hover:bg-white hover:text-[#031446]"
    >
      <p class="text-lg font-semibold">📍Discovery Mall Bali</p>
    </a>

    <!-- title & motto
    <div class="h-full w-full items-center justify-center flex flex-col text-center justify-self-center gap-4">

    </div> -->

    <!-- timer -->
    <div
      class="w-7/10 gap-4 backdrop-blur-md rounded-[10px] p-10 flex md:flex-row flex-col items-center justify-between bg-white/1 shadow-[inset_0_0_2px_1px_rgba(255,255,255,0.25),inset_0_0_10px_3px_rgba(0,0,0,0.25)]"
    >
      <div
        class="md:w-1/4 bg-[radial-gradient(circle,rgba(4,102,200,0.5),transparent,transparent)]"
      >
        <p class="md:text-6xl text-5xl medium">{{ daysRef }}</p>
        <p class="md:text-3xl text-2xl medium">Days</p>
      </div>
      <div
        class="md:w-1/4 bg-[radial-gradient(circle,rgba(4,102,200,0.5),transparent,transparent)]"
      >
        <p class="md:text-6xl text-5xl medium">{{ hoursRef }}</p>
        <p class="md:text-3xl text-2xl medium">Hours</p>
      </div>
      <div
        class="md:w-1/4 bg-[radial-gradient(circle,rgba(4,102,200,0.5),transparent,transparent)]"
      >
        <p class="md:text-6xl text-5xl medium">{{ minutesRef }}</p>
        <p class="md:text-3xl text-2xl medium">Minutes</p>
      </div>
      <div
        class="md:w-1/4 bg-[radial-gradient(circle,rgba(4,102,200,0.5),transparent,transparent)]"
      >
        <p class="md:text-6xl text-5xl medium">{{ secondsRef }}</p>
        <p class="md:text-3xl text-2xl medium">Seconds</p>
      </div>
    </div>
  </section>
</template>
