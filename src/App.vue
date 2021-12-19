<template>
  <header class="px-40 bg-gradient-to-br from-violet-100 via-white to-white">
    <Nav />
    <div class="py-8 flex flex-row justify-between items-center">
      <div class="basis-1/2">
        <h3 class="text-2xl">
          <span class="font-semibold">Hello</span> 👋
        </h3>
        <h1 class="my-4 text-5xl font-bold leading-tight text-violet-500">
          I am Dimas Pangestu
          <br />A Front-End Developer
        </h1>
        <p
          class="text-xl leading-7 font-medium"
        >Currently studying at State Polytechnic of Jember. Interested in frontend development and want to build a career as a frontend developer.</p>
        <div class="mt-8 flex gap-4">
          <BtnSocial
            url="https://www.instagram.com/dimpang_/"
            icon="insta"
            text="dimpang_"
            bg-color="group-hover:bg-red-500"
            shadow-color="hover:shadow-red-500/10"
            text-color="text-red-500"
          />
          <BtnSocial
            url="https://twitter.com/DimasPangestu"
            icon="twitter"
            text="DimasPangestu"
            bg-color="group-hover:bg-sky-500"
            shadow-color="hover:shadow-sky-500/10 hover:w-48"
            text-color="text-sky-500"
            width-hover
          />
          <BtnSocial
            url="https://www.linkedin.com/in/dimpang/"
            icon="linkedin"
            text="dimpang"
            bg-color="group-hover:bg-blue-500"
            shadow-color="hover:shadow-blue-500/10"
            text-color="text-blue-500"
          />
          <BtnSocial
            url="https://github.com/dimpangg"
            icon="github"
            text="dimpangg"
            bg-color="group-hover:bg-black"
            shadow-color="hover:shadow-black/10"
            text-color="text-black"
          />
          <BtnSocial
            url="https://gitlab.com/dimpang"
            icon="gitlab"
            text="dimpang"
            bg-color="group-hover:bg-amber-500"
            shadow-color="hover:shadow-amber-500/10"
            text-color="text-amber-500"
          />
        </div>
      </div>
      <div class="basis-1/2 flex justify-end mr-14">
        <img src="./assets/images/hero-illustration.png" class="w-96 h-96" />
      </div>
    </div>
  </header>

  <div class="mx-40 my-14 gap-12 bg-violet-600 py-12 flex flex-col items-center rounded-2xl">
    <h3 class="text-2xl text-white">
      <span class="font-semibold">Tech i’ve worked with</span> 👨‍💻
    </h3>
    <div class="grid grid-cols-4 gap-8">
      <CardTech title="VueJS" icon="vue" />
      <CardTech title="ReactJS" icon="react" />
      <CardTech title="Tailwind" icon="tailwind" />
      <CardTech title="Bootstrap" icon="bootstrap" />
      <CardTech title="Laravel" icon="laravel" />
      <CardTech title="Vite" icon="vite" />
      <CardTech title="React Native" icon="react" />
    </div>
  </div>
</template>

<script setup>
import Nav from './components/molecules/Nav.vue';
import CardTech from './components/molecules/CardTech.vue';
import BtnSocial from './components/molecules/BtnSocial.vue';
</script>

