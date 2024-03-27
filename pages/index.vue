<script setup>
import BrandImage from '../assets/img/miguel.jpg';
  
useHead({
  title: "Home | miguelbuccat.me"
});
</script>

<template>
  <div class="flex flex-col min-h-[calc(100vh-60px)] justify-center items-center px-6">
    <div class="flex flex-col md:flex-row gap-4 md:gap-20 justify-center md:justify-normal items-center">
      <img :src="BrandImage" width="300" class="shadow-md rounded-2xl"></img>
      <div class="flex flex-col gap-1 items-center md:items-start">
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