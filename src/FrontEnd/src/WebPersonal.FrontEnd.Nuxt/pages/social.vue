<template>
  <main class="min-h-screen">
    <div class="space-y-6 text-center pt-10">
      <h1 class="text-xl font-bold tracking-tight text-gray-800">
        Contact Me
      </h1>
    </div>
    <div class="space-y-6 pt-10">
      <NuxtLink
      v-for="link in links"
      :key="link.icon"
      :to="link.url"
      target="_blank"
      class="flex items-end gap-4 dark:hover:text-gray-300 group">
        <span class="text-sm">
          {{ link.name }}
        </span>
        <div
          class="flex-1 border-b border-dashed border-gray-300 dark:border-gray-800 group-hover:border-gray-700"
        ></div>
        <Icon :name="link.icon" class="w-6 h-6"></Icon>
      </NuxtLink>
    </div>
    
  </main>
</template>
  
<script setup>
// import { Icon } from '@iconify/vue';

  const links = [
    {
      name: "GitHub",
      url: "https://github.com/bautistamangoni",
      icon: "mdi:github",
    },
    {
      name: "Linkedin",
      url: "https://www.linkedin.com/in/juanbautistamangoni/",
      icon: "mdi:linkedin",
    }
  ];

  const description =
    "Here you have all my socials to reach me. Looking forward to meet new people and contribute in projects";
  useSeoMeta({
    title: "Contact me | Juan Bautista Mangoni",
    description,
  });
  
</script>