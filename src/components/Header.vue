<template>
  <header
    class="w-9/10 flex justify-between items-center justify-self-center bg-white/6 shadow-[inset_0_0_1px_1px_rgba(255,255,255,0.35),inset_0_0_10px_1px_rgba(0,0,0,0.25)] backdrop-blur-md rounded-[10px] fixed top-10 pl-10 pr-10 pt-1 pb-1 z-999"
  >
    <a href="#hero" class="flex h-20">
      <img src="/images/logo-bse.png" class="h-full" />
    </a>

    <nav class="md:text-2xl text-base h-15 gap-4 flex font-medium items-center">
      <a href="#about" class="md:flex hidden items-center h-full p-4"><p>About</p></a>
      <a href="#history" class="md:flex hidden items-center h-full p-4"><p>History</p></a>
      <a href="#activity" class="md:flex hidden items-center h-full p-4"><p>Activity</p></a>
      <a href="#side-event" class="md:flex hidden items-center h-full p-4"><p>Side Event</p></a>
      <a href="#gallery" class="md:flex hidden items-center h-full p-4"><p>Gallery</p></a>
      <a
        href="https://docs.google.com/forms/d/e/1FAIpQLSeHGbYsqReE8qbyuMw05qlQxOMBw5D3PD3mqIYmIKd8ILbh1Q/viewform?usp=header"
        target="_blank"
        class="flex items-center h-max p-3 pl-7 pr-7 rounded-3xl bg-linear-to-r bg-[#022894] to-[#031446] cursor-pointer"
        ><p>Register</p></a
      >
    </nav>
  </header>
</template>
