<template>
  <main class="bg-indigo-50">
    <!-- <NuxtLoadingIndicator />
    <NuxtParticles  id="tsparticles"
                    url="assets/particles/particles.json"
                    @load="onLoad"> 
    </NuxtParticles> -->
    <UContainer class="no-padding ">
      <div class="">
        <AppNavbar />
      </div>
      <div class="">
        <NuxtPage />
      </div>
    </UContainer>
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
  width: 20%;
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