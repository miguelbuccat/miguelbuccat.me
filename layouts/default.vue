<script setup>
const mobileMenu = ref(false);
</script>

<template>
  <div class="min-h-screen flex flex-col bg-white">
    <div class="flex flex-row justify-between px-5 md:px-24 py-2 items-center h-[60px]">
      <div class="flex flex-row gap-6 items-center">
        <RouterLink to="/" class="font-light text-xl">miguelbuccat.me</RouterLink>
        <RouterLink to="/" class="hover:text-slate-800 hidden md:block">Home</RouterLink>
        <RouterLink to="/about" class="hover:text-slate-800 hidden md:block">About me</RouterLink>
        <RouterLink to="/projects" class="hover:text-slate-800 hidden md:block">Projects</RouterLink>
        <RouterLink to="/blog" class="hover:text-slate-800 hidden md:block">Blog</RouterLink>
      </div>
      <div class="flex flex-row gap-6 items-center">
        <button class="block md:hidden" @click="() => mobileMenu = !mobileMenu">
          <ChevronDown v-if="!mobileMenu" />
          <ChevronUp v-else />
        </button>
      </div>
    </div>
    <div class="flex-col block md:hidden" v-if="mobileMenu">
      <RouterLink to="/"
        class="transition hover:text-slate-800 hover:bg-slate-50 hover:translate-x-4 block md:hidden px-5 py-3">Home
      </RouterLink>
      <RouterLink to="/about"
        class="transition hover:text-slate-800 hover:bg-slate-50 hover:translate-x-4 block md:hidden px-5 py-3">About me
      </RouterLink>
      <RouterLink to="/projects"
        class="transition hover:text-slate-800 hover:bg-slate-50 hover:translate-x-4 block md:hidden px-5 py-3">Projects
      </RouterLink>
      <RouterLink to="/blog"
        class="transition hover:text-slate-800 hover:bg-slate-50 hover:translate-x-4 block md:hidden px-5 py-3">Blog
      </RouterLink>
    </div>
    <slot />
  </div>
</template>