<template>
  <main>
    <ContentDoc>
      <template #not-found>
        <div class="flex flex-col min-h-[calc(100vh-60px)] justify-center items-center px-6">
          <div class="flex flex-col gap-4 justify-center items-center text-center">
            <h1 class="text-2xl font-semibold">Page not found</h1>
            <p>Could not return the page you were looking for</p>
          </div>
        </div>
      </template>
      <template v-slot="{ doc }">
        <div class="flex flex-col items-center py-4 px-6">
          <article class="prose shadow-md bg-slate-50 rounded-md py-4 px-6">
            <h1>{{ doc.title }}</h1>
            <p class="font-extralight">{{ doc.date }}</p>
            <ContentRenderer :value="doc" />
          </article>
        </div>
      </template>
    </ContentDoc>
  </main>
</template>