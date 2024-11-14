<template>
  <main class="min-h-screen">
    <div class="space-y-6 text-center pt-10">
      <h1 class="text-xl font-bold tracking-tight text-gray-800">
        Contact Me
      </h1>
      <Icon icon="devicon:linkedin-wordmark"  />
      <UButton
        icon="devicon:linkedin-wordmark"
        size="sm"
        color="primary"
        variant="solid"
        label=""
        to="https://www.linkedin.com/in/juanbautistamangoni/" 
        external target="_blank"
        :trailing="false"
      />
      <Icon name="uil:github" style="color: black" />
    </div>
  </main>
</template>
  
<script setup>
import { Icon } from '@iconify/vue';

  const description =
    "I’ve worked on tons of little projects over the years but these are the ones that I’m most proud of. Many of them are open-source, so if you see something that piques your interest, check out the code and contribute if you have ideas for how it can be improved.";
  useSeoMeta({
    title: "Contact me | Juan Bautista Mangoni",
    description,
  });
  
</script>