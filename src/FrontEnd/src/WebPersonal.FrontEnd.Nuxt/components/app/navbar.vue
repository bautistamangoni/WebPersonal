<template>

    <UVerticalNavigation :links="links" 
    :ui="{
      padding: 'p-10 ps-4',
      rounded: '',
      ring: '',
      font: 'text-xl',
    }"
    >
    <template #avatar="{ link }">
      <UAvatar v-if="link.avatar" v-bind="link.avatar" size="xl" loading="lazy" />
    </template>
  </UVerticalNavigation>
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
  // {
  //   label: 'Sobre mí',
  //   icon: 'i-heroicons-home',
  //   to: ''
  // }, 
  {
    label: 'Professional Experience',
    icon: 'i-heroicons-chart-bar',
    to: '/experience'
  }, {
    label: 'Projects',
    icon: 'i-heroicons-command-line',
    to: '/projects'
  }], [{
    label: 'Contact Me',
    icon: 'i-heroicons-light-bulb',
    to: '/social'
  }
  //, {
  //   label: 'Help',
  //   icon: 'i-heroicons-question-mark-circle'
  // }
  ]
]
</script>



