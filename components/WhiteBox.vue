<template>
  <div class="grid-container" mpp grid h-lg w-full overflow-hidden bg-white py-5>
    <div class="grid-item">
      <slot name="left" />
    </div>
    <div class="grid-item">
      <slot name="right" />
    </div>
  </div>
</template>

<style scoped>
.grid-container {
  grid-template-columns: repeat(2, 1fr); /* 创建两列 */
  grid-gap: 1rem; /* 设置元素间隙 */
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
}

.grid-item {
  background-color: #ccc;
  padding: 10px;
}
</style>
