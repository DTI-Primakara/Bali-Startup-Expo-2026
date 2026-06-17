<script setup lang="ts">
import ActivityBox from './ActivityBox.vue'
</script>

<template>
  <section id="activity" class="scroll-m-40 mb-50 pl-20 pr-20 relative">
    <!-- shine decoration -->
    <div
      class="absolute w-150 h-150 rounded-full top-0 -right-70 opacity-50 bg-[radial-gradient(circle,#022894,white)] blur-[200px] -z-100"
    ></div>

    <!-- star decor -->
    <div class="star-1 opacity-66 -rotate-153 w-40 h-40 top-32 right-1 absolute z-50"></div>
    <div class="star-2 rotate-114 w-60 h-60 top-115 -left-10 absolute z-50"></div>

    <div class="mb-15 flex justify-between items-center">
      <div>
        <div class="gap-4 flex items-center">
          <hr class="w-10 border text-[#0466C8]" />
          <p class="text-xl font-bold">Event</p>
        </div>
        <h1 class="text-6xl font-bold">
          Detail <br />
          <p class="bg-[#022894] to-[#0466C8] bg-linear-to-b text-transparent bg-clip-text">
            Activity
          </p>
        </h1>
      </div>

      <p class="text-xl max-w-120 font-medium text-right">
        Figma ipsum component variant main layer. Inspect clip opacity Dolor sit Amet Lorem ipsum
        variant player sit Inspect.
      </p>
    </div>

    <div class="grid gap-10 grid-cols-2 grid-rows-2">
      <!-- <div
        class="w-full h-full gap-2 backdrop-blur-sm rounded-[10px] p-10 flex flex-col justify-center bg-white/15 shadow-[0_0_4px_2px_rgba(255,255,255,0.4)]"
      >
        <h2 class="text-3xl font-semibold">Talkshow Day 1</h2>
        <p class="text-xl mb-4 font-medium text-gray">
          Discover groundbreaking ventures across 100+ booths from the region’s brightest founders
        </p>

        <div class="text-xl font-medium grid gap-2 grid-cols-[1fr_10fr] grid-rows-2 items-center">
          <img src="../assets/images/icon-time.png" />
          <p>: Validation & Market Fit</p>

          <img src="../assets/images/icon-document.png" />
          <p>: 09:00 - 12:00 WITA</p>

          <img src="../assets/images/icon-microphone.png" />
          <p>: I Wayan Indra Adhi Suputra, S.Kom.</p>
        </div> -->
      <ActivityBox
        title="Talkshow Day 1"
        description="Discover groundbreaking ventures across 100+ booths from the region’s brightest founders"
        topic="Validation & Market Fit"
        time="09:00 - 12:00 WITA"
        speaker="I Wayan Indra Adhi Suputra, S.Kom."
      />

      <ActivityBox
        title="Talkshow Day 2"
        description="Discover groundbreaking ventures across 100+ booths from the region’s brightest founders"
        topic="Validation & Market Fit"
        time="09:00 - 12:00 WITA"
        speaker="Putu Surya Sudarmadi, S.Kom."
      />

      <ActivityBox
        title="Sharing Session Day 2"
        description="Discover groundbreaking ventures across 100+ booths from the region’s brightest founders"
        topic="Validation & Market Fit"
        time="09:00 - 12:00 WITA"
        speaker="Agus Yusida, S.Kom."
      />

      <ActivityBox
        title="Sharing Session Day 2"
        description="Discover groundbreaking ventures across 100+ booths from the region’s brightest founders"
        topic="Validation & Market Fit"
        time="09:00 - 12:00 WITA"
        speaker="Agus Yusida, S.Kom."
      />

      <ActivityBox
        title="Sharing Session Day 2"
        description="Discover groundbreaking ventures across 100+ booths from the region’s brightest founders"
        topic="Validation & Market Fit"
        time="09:00 - 12:00 WITA"
        speaker="Putu Evan"
      />
    </div>
  </section>
</template>
