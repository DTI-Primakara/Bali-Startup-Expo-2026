<template>
  <section class="h-screen gap-6 flex flex-col items-center justify-center text-center relative">
    <!-- gradient circle -->
    <div
      class="absolute w-100 h-100 mb-100 rounded-full opacity-50 bg-[radial-gradient(circle,#007FFF,#007FFF)] blur-[150px] -z-100"
    ></div>

    <!-- star decor -->
    <div class="star-1 rotate-45 opacity-20 w-30 h-30 top-0 left-20 absolute -z-50"></div>
    <div class="star-1 rotate-45 opacity-20 w-30 h-30 top-10 left-60 absolute -z-50"></div>
    <div class="star-1 rotate-45 opacity-20 w-30 h-30 -top-10 left-120 absolute -z-50"></div>
    <div class="star-1 rotate-45 opacity-20 w-30 h-30 top-80 left-20 absolute -z-50"></div>
    <div class="star-1 rotate-45 opacity-20 w-20 h-20 top-80 left-60 absolute -z-50"></div>
    <div class="star-1 -rotate-11 w-20 h-20 top-50 left-50 absolute -z-50"></div>

    <div class="star-1 rotate-45 opacity-20 w-30 h-30 -top-10 right-120 absolute -z-50"></div>
    <div class="star-1 rotate-45 opacity-20 w-30 h-30 top-20 right-60 absolute -z-50"></div>
    <div class="star-1 rotate-45 opacity-20 w-30 h-30 top-30 right-20 absolute -z-50"></div>
    <div class="star-1 rotate-45 opacity-20 w-30 h-30 top-70 right-20 absolute -z-50"></div>
    <div class="star-1 rotate-45 opacity-20 w-30 h-30 top-80 right-50 absolute -z-50"></div>
    <div class="star-1 -rotate-11 w-20 h-20 top-55 right-50 absolute -z-50"></div>

    <p class="font-semibold text-sm text-[#164CA4]">FINAL COUNTDOWN</p>
    <p class="font-semibold text-5xl">
      Ready To Launch <br />
      Your Future?
    </p>
    <p class="mb-8 font-medium text-md text-gray">
      Join Bali Startup Expo 2026 and Become Part of Bali’s Innovation
    </p>

    <button
      class="rounded-[50px] p-8 pl-12 pr-12 font-semibold text-xl bg-linear-to-r bg-[#0466C8] to-[#033E79] flex items-center gap-4 cursor-pointer"
    >
      Register Now
      <img class="h-5 w-5" src="../assets/images/right-arrow.png" />
    </button>
  </section>
</template>
