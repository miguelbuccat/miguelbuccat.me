<template>
  <div class="min-h-screen flex flex-col bg-white">
    <div class="flex flex-row justify-between px-5 md:px-24 py-2 items-center h-[60px]">
      <div class="flex flex-row gap-2 items-center">
        <RouterLink to="/" class="font-light text-xl">miguelbuccat.me</RouterLink>
      </div>
    </div>
    <slot />
  </div>
</template>