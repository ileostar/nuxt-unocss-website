<script setup lang="ts">
const typedText = ref('')
onMounted(() => {
  const fullText = 'Welcome to the official website of HCLAB'
  let currentIndex = 0

  const intervalId = setInterval(() => {
    typedText.value += fullText[currentIndex]
    currentIndex++
    if (currentIndex === fullText.length) {
      currentIndex = 0
      clearInterval(intervalId)
    }
  }, 100)
})
</script>

<template>
  <div>
    <p>
      <span v-text="typedText" />
      <span class="cursor" m-l-1 bg-dark dark:bg-white />
    </p>
  </div>
</template>

<style scoped>
.cursor {
  display: inline-block;
  width: 3px;
  height: 16px;
  animation: blink 1s infinite alternate;
}
.cursor.dark {
  display: inline-block;
  width: 3px;
  height: 16px;
  animation: blink 1s infinite alternate;
}

@keyframes blink {
  from {
    opacity: 1;
  }
  to {
    opacity: 0;
  }
}
</style>
