<template>
  <UError
    :clear="{
      color: 'primary',
      size: 'xl',
      icon: 'i-lucide-arrow-left',
      class: 'rounded-full transition duration-400 ease-in-out bg-primary hover:bg-green-700 transform hover:-translate-y-1 hover:scale-110'
    }"
    :error="{
      statusCode: 404,
      statusMessage: 'Page not found',
      message: 'The page you are looking for does not exist.'
    }"
  />
</template>
  