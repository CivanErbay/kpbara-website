<template>
  <main
    class="grid lg:grid-cols-2 place-items-center pt-16 pb-8 md:pt-8"
  >
    <div class="p-24 md:order-1 hidden md:block">
      <img
        class="rounded-full transition-transform transform hover:scale-125"
        src="~/assets/img/hero.jpeg"
        alt="Starship starts the engine"
        loading="eager"
        format="avif"
        width="512"
        height="512"
      />
    </div>

    <div>
      <h1
        class="text-5xl lg:text-6xl xl:text-6xl !leading-[1.1] font-bold lg:tracking-tight"
      >
        Turning innovation into intelligent solutions.
      </h1>
      <p class="text-lg mt-4 text-slate-600 max-w-xl">
        Empowering your vision with cutting-edge AI technology, we
        bring your ideas to life with precision, creativity, and
        innovation.
      </p>
     <!--  <div class="mt-6 flex flex-col sm:flex-row gap-3">
        <LandingLink
          href="https://github.com/Gr33nW33n/nuxtship-template"
          target="_blank"
          rel="noopener"
          >Get Started</LandingLink
        >
        <LandingLink
          size="lg"
          styleName="outline"
          rel="noopener"
          href="https://github.com/Gr33nW33n/nuxtship-template"
          target="_blank"
          >View Repo</LandingLink
        >
      </div> -->
    </div>
  </main>
</template>
