<script setup lang="ts">
import HeaderComp from '~/components/HeaderComp.vue';
</script>

<template>
    <UApp>
        <HeaderComp />
        <slot />
    </UApp>
  </template>
