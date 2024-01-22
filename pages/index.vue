<script setup lang="ts">
definePageMeta({
  layout: 'home',
})
</script>

<template>
  <div>
    <Suspense>
      <Banner />
      <template #fallback>
        <div italic op50>
          <span animate-pulse>Loading...</span>
        </div>
      </template>
    </Suspense>
    <Wavy />
    <FeatureBox/>
    <GreyBox />
    <Direction/>
  </div>
</template>
