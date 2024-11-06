<template>
  <main class="min-h-screen">
    <div>
      <HomeIntro />
    </div>
    <div class="space-y-6 text-center pt-10">
      <UButton
        icon="i-heroicons-arrow-down-circle-16-solid"
        size="sm"
        color="primary"
        variant="solid"
        label="Download CV"
        to="/curriculum/MangoniJuanBautistaCV.pdf" 
        external target="_blank"
        :trailing="false"
      />
    </div>
  </main>
</template>

<script setup>
  const description =
    "I’ve worked on tons of little projects over the years but these are the ones that I’m most proud of. Many of them are open-source, so if you see something that piques your interest, check out the code and contribute if you have ideas for how it can be improved.";
  useSeoMeta({
    title: "Juan Bautista Mangoni",
    description,
  });

</script>

