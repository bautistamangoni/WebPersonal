<template>
<div class="flex top-0 w-full z-50">
  <UHorizontalNavigation  :links="links" 
    :ui="{
      rounded: '',
      ring: '',
      font: 'text-l'
    }"
    >
    <template #avatar="{ link }">
      <UAvatar v-if="link.avatar" v-bind="link.avatar" size="xs" loading="lazy" />
    </template>
  </UHorizontalNavigation>
</div>

</template>

<script setup lang="ts">
import type { _maxWidth } from '#tailwind-config/theme';

const links = [
  [{
    label: 'Juan Bautista Mangoni',
    avatar: {
      src: 'https://avatars.githubusercontent.com/u/183560782?v=4'
    },
    to: '/'
  }, 
  {
    label: '',
    icon: 'i-heroicons-chart-bar',
    to: '/experience'
  }
  // , {
  //   label: '',
  //   icon: 'i-heroicons-command-line',
  //   to: '/projects'
  // },
  // {
  //   label: '',
  //   icon: 'i-heroicons-users',
  //   to: '/social'
  // }
  ]
]
</script>



