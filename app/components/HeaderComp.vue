<script setup lang="ts">
import type { NavigationMenuItem } from '@nuxt/ui'

const route = useRoute()

const items = computed<NavigationMenuItem[]>(() => [{
  label: 'Available Games',
  to: '/games',
  active: route.path.startsWith('/games')
}, {
  label: 'Pricing Plans',
  to: '/pricing',
  active: route.path.startsWith('/pricing')
}, {
  label: 'About',
  to: '/about',
  active: route.path.startsWith('/about')
}])
</script>

<template>   
  <UHeader title="Best Game Store">
      <UNavigationMenu :items="items" />
      <template #right>
        <UColorModeButton />
        <UButton
          color="neutral"
          variant="ghost"
          to="https://github.com/HardCodeDev777/TestNuxtGameStore"
          target="_blank"
          icon="i-simple-icons-github"
          aria-label="GitHub"
        />
      </template>
  </UHeader>
</template>
