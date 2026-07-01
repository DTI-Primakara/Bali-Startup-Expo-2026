<script setup lang="ts">
import { motion } from 'motion-v'
import ActivityBox from './ActivityBox.vue'
</script>

<template>
  <section id="activity" class="scroll-m-40 mb-50 md:pl-20 md:pr-20 pl-10 pr-10 relative">
    <!-- shine decoration -->
    <div
      class="absolute w-150 h-150 rounded-full top-0 -right-70 opacity-50 bg-[radial-gradient(circle,#022894,white)] blur-[200px] -z-100"
    ></div>

    <!-- star decor -->
    <div class="star-1 opacity-66 -rotate-153 w-40 h-40 top-32 right-1 absolute z-50"></div>
    <div class="star-2 rotate-114 w-60 h-60 top-115 -left-10 absolute z-50"></div>

    <div class="mb-15 flex md:flex-row flex-col justify-between items-center">
      <motion.div
        :initial="{ y: 100, opacity: 0 }"
        :while-in-view="{ y: 0, opacity: 1 }"
        :transition="{ duration: 0.4 }"
        :in-view-options="{ once: true }"
      >
        <div class="gap-4 flex md:flex-row flex-col items-center">
          <hr class="w-10 border text-[#0466C8] md:block hidden" />
          <p class="md:text-xl text-base font-bold">Event</p>
        </div>
        <h1 class="md:text-6xl text-4xl font-bold md:text-left text-center">
          Detail <br />
          <p class="bg-[#022894] to-[#0466C8] bg-linear-to-b text-transparent bg-clip-text">
            Activity
          </p>
        </h1>
      </motion.div>

      <motion.p
        :initial="{ y: 100, opacity: 0 }"
        :while-in-view="{ y: 0, opacity: 1 }"
        :transition="{ duration: 0.4 }"
        :in-view-options="{ once: true }"
        class="md:text-xl text-base max-w-120 font-medium md:text-right text-center"
      >
        Jangan lewatkan kesempatan emas belajar langsung dari para praktisi dan founder sukses
        lokal. Temukan strategi jitu membangun bisnis dari nol hingga siap bersaing secara global.
      </motion.p>
    </div>

    <div class="md:grid flex flex-col gap-10 grid-cols-2 justify-center items-center">
      <!-- <div
        class="w-full h-full gap-2 backdrop-blur-sm rounded-[10px] p-10 flex flex-col justify-center bg-white/15 shadow-[0_0_4px_2px_rgba(255,255,255,0.4)]"
      >
        <h2 class="text-3xl font-semibold">Talkshow Day 1</h2>
        <p class="text-xl mb-4 font-medium text-gray">
          Discover groundbreaking ventures across 100+ booths from the region’s brightest founders
        </p>

        <div class="text-xl font-medium grid gap-2 grid-cols-[1fr_10fr] grid-rows-2 items-center">
          <img src="/images/icon-time.png" />
          <p>: Validation & Market Fit</p>

          <img src="/images/icon-document.png" />
          <p>: 09:00 - 12:00 WITA</p>

          <img src="/images/icon-microphone.png" />
          <p>: I Wayan Indra Adhi Suputra, S.Kom.</p>
        </div> -->
      <ActivityBox
        title="Talkshow Day 1"
        description="Diskusi interaktif mengenai tantangan nyata dan masa depan startup di Pulau Dewata"
        topic="Startup di Pulau Dewata: Antara Peluang Global dan Tantangan Nyata"
        time="19:05 - 19:50 WITA"
        speaker="Putu Surya Sudarmadi (Owner GuestPro) & I Wayan Indra Adhi Suputra, S.Kom. (CEO Djoin)"
      />

      <ActivityBox
        title="Sharing Session Day 2"
        description="Belajar strategi digital branding untuk mengubah cerita produk menjadi konversi penjualan"
        topic="Jual Cerita, Bukan Cuma Produk: Strategi Digital Branding untuk Bisnis Kreatif"
        time="15:40 - 16:40 WITA"
        speaker="Putu Evananda (Wasana Bali)"
      />

      <ActivityBox
        title="Sharing Session Day 2"
        description="Strategi taktis memasarkan jasa IT secara tepat sasaran ke pelaku bisnis lokal"
        topic="Jual Solusi, Bukan Sekadar Fitur: Strategi Branding Jasa IT untuk Menyasar Market Lokal"
        time="16:10 - 16:40 WITA"
        speaker="Merta Yoga (Atrem Project)"
      />

      <ActivityBox
        title="Light Talk Day 2"
        description="Mengulik realita di balik sustainable business yang membawa dampak nyata bagi lingkungan"
        topic="Profit with Purpose: Realita Menjalankan Bisnis yang Berdampak pada Lingkungan"
        time="17:10 - 17:50 WITA"
        speaker="I Made Wisakananda Pradipta"
      />
    </div>
  </section>
</template>
