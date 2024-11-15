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
  const description = "I am a .NET software developer with experience in back-end and front-end development for banking/financial";
  useSeoMeta({
    title: "Juan Bautista Mangoni",
    description,
  });

</script>

