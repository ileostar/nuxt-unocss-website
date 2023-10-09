<template>
  <div class="grid-container" mpp h-50 flex justify-between overflow-hidden>
    <div class="grid-item" flex="~ col 1" items-center>
      <div flex="~ col 1" w-sm items-start justify-center>
        <Logos mb-6 />
        <ClientOnly>
          <Type animate-pulse op50 />
          <template #fallback>
            <div op50>
              <span animate-pulse>Hi...</span>
            </div>
          </template>
        </ClientOnly>
      </div>
    </div>
    <div class="grid-item" flex-1 />
  </div>
</template>

<style scoped>
.grid-container {
  grid-template-columns: repeat(2, 1fr); /* 创建两列 */
  grid-gap: 1rem; /* 设置元素间隙 */
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
}

.grid-item {
  padding: 10px;
}
</style>
