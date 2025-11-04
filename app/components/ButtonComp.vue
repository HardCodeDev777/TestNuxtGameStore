<script setup lang="ts">
defineProps<{
  label: string,
  to: string,
  icon: string
}>()
</script>

<template>
  <UButton 
  class="btn-animated" 
  :to="to" size="xl" color="primary" :icon="icon">
    {{ label }}
  </UButton>
</template>