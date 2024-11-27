<template>
  <main class="bg-slate-50 font-mono">
    <!-- <NuxtLoadingIndicator />
    <NuxtParticles  id="tsparticles"
                    url="assets/particles/particles.json"
                    @load="onLoad"> 
    </NuxtParticles> -->
    
    <div class="h-32"></div>
    <UContainer class="">
      <AppNavbar />
        <NuxtPage />
        <AppSocials />
    </UContainer>
    <div class="h-32"></div>
    
    <AppFooter/>
  </main>
</template>

<script setup lang="ts">
  import type { Container } from '@tsparticles/engine'
  
  const onLoad = (container: Container) => {
    container.pause()
    setTimeout(() => container.play(), 1000)
  }
</script>

<style scoped>
.flex {
  display: flex;
}

.no-padding {
  padding: 0;
}

.navbar{
  height: 100vh;
  top:0;
  position: fixed;

}

.flex-grow {
  flex-grow: 1;
}

.main-content {
  width: 100%;
  top:20;
}

</style>