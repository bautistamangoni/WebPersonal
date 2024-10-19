<template>
    <UVerticalNavigation :links="links" />
</template>

<script setup lang="ts">
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
    label: 'Ejemplos',
    icon: 'i-heroicons-light-bulb'
  }
  //, {
  //   label: 'Help',
  //   icon: 'i-heroicons-question-mark-circle'
  // }
  ]
]
</script>



