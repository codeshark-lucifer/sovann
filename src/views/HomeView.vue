<template>
  <section id="Home" class="px-4 py-16 md:px-10 lg:px-40">
    <div class="mx-auto grid max-w-6xl items-center gap-10 md:grid-cols-2">
      <div class="space-y-6 text-slate-800">
        <p class="text-sm font-semibold uppercase tracking-[0.25em] text-slate-500">Hello there</p>
        <h3 class="text-2xl font-semibold md:text-4xl">Hi, I'm <span class="text-emerald-700">SOVANN</span></h3>
        <h1 class="text-5xl font-black leading-none tracking-tight md:text-7xl">I'm a Web Developer</h1>
        <p class="max-w-xl text-lg font-medium text-slate-600">I'm a senior front-end web developer creating clean, modern, and user-friendly digital experiences.</p>
        <div class="flex flex-wrap items-center gap-4 pt-2">
          <RouterLink
            class="rounded-md border border-slate-800 bg-slate-800 px-5 py-3 text-base font-semibold text-white transition hover:bg-slate-700 hover:text-white"
            to="/#About"
          >
            View My Projects
          </RouterLink>
          <a
            href="#About"
            class="rounded-md border border-slate-300 bg-white px-5 py-3 text-base font-semibold text-slate-700 transition hover:border-slate-800 hover:text-slate-900"
          >
            About Me
          </a>
        </div>
      </div>

      <div class="flex justify-center md:justify-end">
        <div class="rounded-3xl border border-slate-200 bg-gradient-to-br from-emerald-50 to-white p-6 shadow-lg shadow-slate-200/60">
          <img class="w-72 drop-shadow-xl md:w-80" src="/favicon.svg" alt="Sovann profile illustration" />
        </div>
      </div>
    </div>
  </section>

  <div class="mx-auto my-6 flex w-full max-w-md items-center px-4">
    <div class="h-px flex-1 bg-slate-300"></div>
    <span class="mx-4 text-sm font-bold uppercase tracking-[0.2em] text-slate-600">About me</span>
    <div class="h-px flex-1 bg-slate-300"></div>
  </div>

  <section id="About" class="px-4 py-10 md:px-10 lg:px-40">
    <div class="mx-auto grid max-w-6xl gap-10 md:grid-cols-2">
      <div class="space-y-5 rounded-xl bg-white p-8 shadow-sm shadow-slate-200/60">
        <p class="text-sm font-semibold uppercase tracking-[0.25em] text-emerald-600">Bonjour!</p>
        <h2 class="text-3xl font-bold text-slate-900">Creative, curious, and detail-driven</h2>
        <p class="text-lg leading-8 text-slate-600">
          I am a self-taught graphic designer and front-end web developer based in Cambodia with extensive
          marketing and communication experience. I am currently studying Information Technology and building a
          strong foundation in modern web design and development.
        </p>

        <div class="pt-2">
          <button class="rounded-full bg-emerald-600 px-5 py-3 text-sm font-semibold text-white transition hover:bg-emerald-700">
            Find Me
          </button>
        </div>

        <ul class="flex flex-wrap gap-3 pt-2 text-sm font-medium text-slate-700">
          <li class="rounded-full border border-slate-200 bg-slate-50 px-3 py-2">Facebook</li>
          <li class="rounded-full border border-slate-200 bg-slate-50 px-3 py-2">Telegram</li>
        </ul>
      </div>

      <div class="rounded-3xl bg-[#2d4635] p-8 text-white shadow-xl shadow-slate-300/40 md:p-10">
        <h2 class="mb-8 text-3xl font-bold tracking-wide text-amber-400">Education</h2>

        <div class="relative space-y-8 pl-6 before:absolute before:bottom-3 before:left-[7px] before:top-2 before:w-[2px] before:bg-white/30">
          <div class="relative flex items-start">
            <span class="absolute -left-6 top-0 select-none text-lg text-[#e06543]">✦</span>
            <div class="grid grid-cols-[110px_1fr] gap-4 items-baseline">
              <span class="font-serif text-lg font-bold text-amber-100/90">2022-2023</span>
              <div>
                <h3 class="font-semibold leading-tight text-white">Digital Campus, Montpellier</h3>
                <p class="mt-1 text-sm text-emerald-100/70">Digital Web & Project Management</p>
              </div>
            </div>
          </div>

          <div class="relative flex items-start">
            <span class="absolute -left-6 top-0 select-none text-lg text-[#e06543]">✦</span>
            <div class="grid grid-cols-[110px_1fr] gap-4 items-baseline">
              <span class="font-serif text-lg font-bold text-amber-100/90">2021-2022</span>
              <div>
                <h3 class="font-semibold leading-tight text-white">IUT de Béziers</h3>
                <p class="mt-1 text-sm text-emerald-100/70">Commercialisation Technique</p>
              </div>
            </div>
          </div>

          <div class="relative flex items-start">
            <span class="absolute -left-6 top-0 select-none text-lg text-[#e06543]">✦</span>
            <div class="grid grid-cols-[110px_1fr] gap-4 items-baseline">
              <span class="font-serif text-lg font-bold text-amber-100/90">2017-2020</span>
              <div>
                <h3 class="font-semibold leading-tight text-white">Economic University, Danang</h3>
                <p class="mt-1 text-sm text-emerald-100/70">International Business</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
