<template>
  <section class="mb-50 pl-20 pr-20 flex flex-col items-center">
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

      <h1 class="text-outline-2 text-6xl font-bold">Special Perform</h1>
    </div>

    <div
      class="w-full gap-2 backdrop-blur-sm rounded-[10px] p-10 flex flex-col justify-center bg-white/15 shadow-[0_0_4px_2px_rgba(255,255,255,0.4)]"
    >
      <div class="gap-10 grid grid-cols-2">
        <div class="w-full h-90 bg-red-500"></div>
        <div class="w-full flex flex-col justify-center">
          <div class="w-fit mb-4 relative">
            <!-- border decoration -->
            <div
              class="h-6 w-20 border-white border-l-2 border-t-2 absolute -top-0.5 -left-3 rounded-tl-sm blur-md"
            ></div>
            <div
              class="h-6 w-20 border-white border-l-2 border-t-2 absolute -top-0.5 -left-3 rounded-tl-sm"
            ></div>

            <div
              class="h-6 w-20 border-white border-r-2 border-b-2 absolute -bottom-0.5 -right-3 rounded-br-sm blur-md"
            ></div>
            <div
              class="h-6 w-20 border-white border-r-2 border-b-2 absolute -bottom-0.5 -right-3 rounded-br-sm"
            ></div>

            <h2 class="text-outline-2 text-3xl font-bold">Special Perform</h2>
          </div>

          <p class="mb-8 font-medium text-xl">
            Figma ipsum component variant main layer. Inspect clip opacity effect style invite
            export. Polygon pixel team layout hand inspect team.
          </p>

          <div class="grid-cols-[1fr_10fr] gap-y-2 grid items-center">
            <img src="../assets/images/icon-calender.png" />
            <p class="text-base font-medium">10 Juli 2026</p>

            <img src="../assets/images/icon-time.png" />
            <p class="text-base font-medium">10:00-11:00 WITA</p>

            <img src="../assets/images/icon-location.png" />
            <p class="text-base font-medium">Discovery Mall</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
