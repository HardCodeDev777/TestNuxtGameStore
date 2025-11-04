<script setup lang="ts">
import ButtonComp from '~/components/ButtonComp.vue';

const plans = ref([
  {
    title: 'Basic',
    description: 'For a short time spent.',
    price: '$4.99',
    features: [
      'Choose any 3 games in a month to play',
      'For each game 5 hours in month'
    ],
    button: {
      label: 'Buy now',
      to: "/about",
      class: "btn-animated"
    }
  },
  {
    title: 'Universal',
    description: 'For usual gamers.',
    price: '$25.99',
    features: [
      'Choose any 10 games in a month to play',
      'For each game 15 hours in month'
    ],
    button: {
      label: 'Buy now',
      to: "/about",
      class: "btn-animated"
    }
  },
  {
    title: 'Premium',
    description: 'For true gamers.',
    price: '$99.99',
    features: [
      'Choose any available game to play',
      'Unlimited time of playing'
    ],
    button: {
      label: 'Buy now',
      to: "/about",
      class: "btn-animated"
    }
  }
])
</script>

<template>
    <UContainer class="flex flex-col justify-center items-center lg:gap-14 p-45">
        <UPricingPlans :plans="plans" />
        <ButtonComp label="See availabe games" to="/games" icon="i-heroicons-squares-2x2"/>
    </UContainer>
</template>
