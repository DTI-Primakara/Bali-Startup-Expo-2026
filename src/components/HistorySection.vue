<script setup lang="ts">
import HistoryBox from './HistoryBox.vue'
import { motion } from 'motion-v'
</script>

<template>
  <section
    id="history"
    class="w-full scroll-m-20 gap-8 mb-30 pt-20 flex flex-col text-center items-center relative md:pl-20 pl-10 md:pr-20 pr-10"
  >
    <div class="relative">
      <!-- border decoration -->
      <div
        class="h-6 w-20 border-white border-l-2 border-t-2 absolute -top-2 -left-3.5 rounded-tl-sm blur-md"
      ></div>
      <div
        class="h-6 w-20 border-white border-l-2 border-t-2 absolute -top-2 -left-3.5 rounded-tl-sm"
      ></div>

      <div
        class="h-6 w-20 border-white border-r-2 border-b-2 absolute -bottom-2 -right-3.5 rounded-br-sm blur-md"
      ></div>
      <div
        class="h-6 w-20 border-white border-r-2 border-b-2 absolute -bottom-2 -right-3.5 rounded-br-sm"
      ></div>

      <motion.h1
        :initial="{ y: 100, opacity: 0 }"
        :while-in-view="{ y: 0, opacity: 1 }"
        :transition="{ duration: 0.4 }"
        :in-view-options="{ once: true }"
        class="text-outline-2 md:text-6xl text-4xl font-bold"
        >History of BSE</motion.h1
      >
    </div>

    <motion.p
      :initial="{ y: 100, opacity: 0 }"
      :while-in-view="{ y: 0, opacity: 1 }"
      :transition="{ duration: 0.4 }"
      :in-view-options="{ once: true }"
      class="md:text-xl text-base w-9/10 mb-10 font-medium"
    >
      Konsistensi yang melahirkan dampak. Lihat bagaimana langkah kecil kami kini telah
      bertransformasi menjadi salah satu event teknologi tahunan yang paling dinanti di Bali.
    </motion.p>

    <!-- shine decoration -->
    <div
      class="absolute w-150 h-150 rounded-full top-130 -right-70 opacity-50 bg-[radial-gradient(circle,#022894,white)] blur-[200px] -z-100"
    ></div>

    <!-- star decor -->
    <div class="star-1 opacity-30 rotate-45 w-25 h-25 top-120 right-10 absolute -z-50"></div>
    <div class="star-1 opacity-30 rotate-45 w-25 h-25 top-170 right-70 absolute -z-50"></div>
    <div class="star-1 opacity-30 rotate-45 w-30 h-30 top-310 left-20 absolute -z-50"></div>
    <div class="star-1 opacity-30 rotate-45 w-30 h-30 top-350 right-30 absolute -z-50"></div>
    <div class="star-2 w-50 h-50 top-120 right-75 absolute -z-50"></div>
    <div class="star-2 w-50 h-50 top-170 left-10 absolute -z-50"></div>
    <div class="star-2 rotate-27 opacity-20 w-50 h-50 top-230 left-40 absolute -z-50"></div>
    <div class="star-2 rotate-34 w-50 h-50 top-290 left-70 absolute -z-50"></div>
    <div class="star-2 rotate-15 w-50 h-50 top-320 right-90 absolute -z-50"></div>
    <div class="star-2 rotate-169 w-50 h-50 bottom-10 right-0 absolute -z-50"></div>
    <div class="star-2 rotate-15 w-50 h-50 bottom-0 right-70 absolute -z-50"></div>

    <!-- rocket decor -->
    <div class="rocket w-40 h-40 bottom-50 right-40 absolute -z-50"></div>

    <!-- moon decor -->
    <div class="moon w-20 h-20 top-90 right-60 absolute -z-50"></div>

    <HistoryBox
      :mirrored="false"
      year="2015"
      title="Awal Mula Langkah Kecil"
      description="Berdiri sejak tahun 2015, Bali Startup Expo lahir dari sebuah visi sederhana: memberikan ruang bagi anak muda Bali untuk berani berinovasi di bidang teknologi. Dimulai sebagai wadah internal, benih-benih technopreneurship mulai disemaikan di sini."
    />
    <HistoryBox
      :mirrored="true"
      year="2016 - 2025"
      title="Konsistensi & Pertumbuhan"
      description="BSE konsisten hadir setiap tahun memperluas kolaborasi dengan universitas, pemerintah, dan komunitas nasional seperti 1001 Startup. Didukung rekam jejak yang sukses menarik perhatian khalayak ramai , event ini telah bertransformasi menjadi agenda teknologi tahunan yang paling dinanti di Bali."
    />
    <HistoryBox
      :mirrored="false"
      year="2025 "
      title="Menuju Inovasi Tanpa Batas"
      description='Mengusung tema "From Small Step to Galaxy Innovation," BSE 2025 melibatkan 35 tim (175 mahasiswa) Primakara University. Menghadirkan pameran startup, pitching investor , Coswalk Festival , hingga MLBB Tournament , event ini siap menarik 500+ pengunjung per hari serta memperkuat branding ekosistem digital di Bali.'
    />
  </section>
</template>
