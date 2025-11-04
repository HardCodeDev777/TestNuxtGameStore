<script setup lang="ts">
import ButtonComp from '~/components/ButtonComp.vue';
</script>

<template>
    <UContainer class="flex flex-col justify-center items-center text-center lg:gap-9 p-75">
      <div>
        <h1 class="text-7xl font-bold">Best Games For Best Prices</h1>
      </div>
      <ButtonComp label="See prices" to="/pricing" icon="i-heroicons-arrow-right"/>
    </UContainer>
</template>
  