<script setup lang="ts">
import { appName } from '~/constants'

useHead({
  title: appName,
})
</script>

<template>
  <VitePwaManifest />
  <NuxtLayout>
    <NuxtPage />
  </NuxtLayout>
</template>

<style>
::-webkit-scrollbar {
  display: none;
}
html, body , #__nuxt{
  height: 100vh;
  margin: 0;
  padding: 0;
  scrollbar-width: none;
}
html {
  background: #f0f7ff;
}
html.dark {
  background: #070081;
  color: white;
}
</style>
