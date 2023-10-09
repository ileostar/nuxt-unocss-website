<template>
  <a-layout h-full>
    <a-layout-header mpp>
      <Header />
    </a-layout-header>
    <a-layout-content py-20 text-center>
      <slot />
    </a-layout-content>
    <a-layout-footer>
      <Footer />
    </a-layout-footer>
  </a-layout>
</template>
