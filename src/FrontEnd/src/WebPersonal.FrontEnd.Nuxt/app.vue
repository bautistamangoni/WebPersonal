<template>
  <NuxtLoadingIndicator />
  <UContainer class="flex no-padding">
    <div class="navbar">
      <AppNavbar />
    </div>
    <div class="flex-grow main-content">
      <NuxtPage />
    </div>
  </UContainer>
  <AppFooter />
</template>

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
  left:0;
  position: fixed;

}

.flex-grow {
  flex-grow: 1;
}

.main-content {
  margin-left: 20%; 
  padding: 1rem; 
  width: 100%;
}

</style>