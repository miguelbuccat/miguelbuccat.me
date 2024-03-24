<script setup>
  import BrandImage from '../assets/img/miguel.jpg';
</script>

<template>
  <div class="flex flex-col min-h-screen justify-center items-center px-6">
    <div class="flex flex-row gap-20 items-center flex-wrap">
      <img :src="BrandImage" width="300" class="shadow-md rounded-2xl"></img>
      <div class="flex flex-col gap-1">
        <h1 class="font-extrabold text-3xl">
          Hi! I'm Miguel
        </h1>
        <p>I'm a 16 year old Filipino web developer</p>
        <div class="flex flex-row gap-2">
          <RouterLink class="transition bg-blue-500 hover:bg-blue-700 hover:translate-y-2 px-2 py-1 shadow-md text-white font-bold" to="/about">About me</RouterLink>
          <RouterLink class="transition bg-green-500 hover:bg-green-700 hover:translate-y-2 px-2 py-1 shadow-md text-white font-bold" to="/projects">Projects</RouterLink>
        </div>
      </div>
    </div>
  </div>
</template>