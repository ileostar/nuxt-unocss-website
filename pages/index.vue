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
    <WhiteBox class="-mt">
      <template #left>
        <div bg-blue>
          left
        </div>
      </template>
      <template #right>
        <div bg-blue>
          right
        </div>
      </template>
    </WhiteBox>
    <GreyBox />
    <WhiteBox>
      <template #left>
        <div bg-blue>
          left
        </div>
      </template>
      <template #right>
        <div bg-blue>
          right
        </div>
      </template>
    </WhiteBox>
  </div>
</template>
