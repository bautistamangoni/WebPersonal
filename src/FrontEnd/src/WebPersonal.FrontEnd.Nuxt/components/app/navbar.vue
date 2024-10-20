<template>

    <UVerticalNavigation :links="links" 
    :ui="{
      // wrapper: 'border-s border-gray-200 dark:border-gray-800 space-y-2',
      // base: 'group block border-s -ms-px leading-6 before:hidden',
      padding: 'p-10 ps-4',
      rounded: '',
      ring: '',
      font: 'text-xl', 
     
    
      // active: 'text-primary-500 dark:text-primary-400 border-current font-semibold',
      // inactive: 'border-transparent hover:border-gray-400 dark:hover:border-gray-500 text-gray-700 hover:text-gray-900 dark:text-gray-400 dark:hover:text-gray-300'
    }"
    />
</template>

<script setup lang="ts">
import type { _maxWidth } from '#tailwind-config/theme';

const links = [
  [{
    label: 'Juan Bautista Mangoni',
    avatar: {
      src: 'https://avatars.githubusercontent.com/u/183560782?v=4'
    },
    badge: 100
  }, {
    label: 'Sobre mí',
    icon: 'i-heroicons-home',
    to: '/getting-started/installation'
  }, {
    label: 'Experiencia profesional',
    icon: 'i-heroicons-chart-bar',
    to: '/components/vertical-navigation'
  }, {
    label: 'Proyectos',
    icon: 'i-heroicons-command-line',
    to: '/components/command-palette'
  }], [{
    label: 'Contacto',
    icon: 'i-heroicons-light-bulb'
  }
  //, {
  //   label: 'Help',
  //   icon: 'i-heroicons-question-mark-circle'
  // }
  ]
]
</script>



