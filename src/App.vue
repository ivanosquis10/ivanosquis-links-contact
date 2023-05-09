<script setup>
import Links from './components/Links.vue'
import BgAnimated from './components/BgAnimated.vue'
import Footer from './components/Footer.vue'
</script>

<template>
  <BgAnimated />
  <main
    class="w-full h-screen flex flex-col items-center justify-around relative"
  >
    <h1
      class="
        text-white
        font-bold
        text-2xl
        md:text-5xl
        text-center
        p-4
        rounded-2xl
        sticky
        backdrop-blur-3xl
        bg-slate-800/30
      "
    >
      Ivanosquis Links Contact
    </h1>

    <section class="w-full md:w-1/2 mx-auto p-2">
      <Links />
    </section>
    <Footer />
  </main>
</template>
