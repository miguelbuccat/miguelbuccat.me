<script setup>
const posts = await queryContent('blog').find();

console.log(posts)
</script>

<template>
  <div class="flex flex-col justify-center items-center min-h-[500px] gap-2 px-8">
    <h1 class="text-3xl font-bold">Blog</h1>
    <p class="font-light">A place for my ideas, rants, and just about anything I can talk about</p>
  </div>
  <div class="flex flex-col gap-2 justify-center items-center py-4 px-6">
    <RouterLink class="flex flex-col md:min-w-[400px] bg-slate-50 transition hover:scale-110 focus:scale-90 py-4 px-6 gap-1" v-for="post of posts" :to="post._path">
      <h1 class="text-3xl font-bold">{{ post.title }}</h1>
      <p class="font-light">{{ post.excerpt }}</p>
      <p class="mt-4">{{ post.date }}</p>
    </RouterLink>
  </div>
</template>