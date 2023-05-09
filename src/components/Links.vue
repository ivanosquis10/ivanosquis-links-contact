<script setup>
const links = [
  {
    id: 1,
    social: '@Ivanosquis13',
    url: 'https://twitter.com/ivanosquis13',
    icon: './twitter.svg',
  },
  {
    id: 2,
    social: 'Ivanosquis10',
    url: 'https://github.com/ivanosquis10',
    icon: './github.svg',
  },
  {
    id: 3,
    social: 'my portfolio!',
    url: 'https://portfolio-ivanosquis-iv.vercel.app/',
    icon: './web.svg',
  },
  {
    id: 3,
    social: 'About me!',
    url: 'https://read.cv/ivanosquis13',
    icon: './info.svg',
  },
]
</script>

<template>
  <ul class="relative space-y-5">
    <li
      v-for="{ id, social, url, icon } in links"
      :key="id"
      class="
        flex
        justify-between
        items-center
        gap-2
        text-white
        p-4
        rounded-lg
        sticky
        backdrop-blur-3xl
        bg-slate-900/50
        duration-300
        ease-in-out
        hover:bg-gray-800/40
        shadow-xl
      "
    >
      <img
        width="44"
        height="44"
        :src="icon"
        alt="imagen relacionada con el logo de la red social"
        loading="lazy"
      />

      <p class="text-base md:text-xl uppercase font-bold">{{ social }}</p>

      <a
        :href="url"
        aria-label="icono de enlace para ir a una red social"
        target="_blank"
      >
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="
            icon icon-tabler icon-tabler-link
            transform
            hover:scale-125
            duration-300
            ease-in-out
          "
          width="44"
          height="44"
          viewBox="0 0 24 24"
          stroke-width="2"
          stroke="#ffffff"
          fill="none"
          stroke-linecap="round"
          stroke-linejoin="round"
        >
          <path stroke="none" d="M0 0h24v24H0z" fill="none" />
          <path d="M10 14a3.5 3.5 0 0 0 5 0l4 -4a3.5 3.5 0 0 0 -5 -5l-.5 .5" />
          <path
            d="M14 10a3.5 3.5 0 0 0 -5 0l-4 4a3.5 3.5 0 0 0 5 5l.5 -.5"
          /></svg
      ></a>
    </li>
  </ul>
</template>
