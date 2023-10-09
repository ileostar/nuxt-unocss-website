<template>
  <div text="xl gray4" m-5 flex="~ gap3" items-center justify-between>
    <div class="logo">
      <img src="/favicon.ico" alt="">
    </div>
    <ul class="menu" flex gap-6 overflow-hidden text-base>
      <li hover:color-blue>
        <NuxtLink to="/">
          HOME
        </NuxtLink>
      </li>
      <li hover:color-blue>
        <NuxtLink to="/team">
          TEAM
        </NuxtLink>
      </li>
      <li hover:color-blue>
        <NuxtLink to="/product">
          PRODUCT
        </NuxtLink>
      </li>
      <li hover:color-blue>
        <NuxtLink to="/join">
          JOIN
        </NuxtLink>
      </li>
      <li hover:color-blue>
        <NuxtLink to="http://js.hclab.cn">
          TIME
        </NuxtLink>
      </li>
    </ul>
    <div class="logo">
      <img src="/favicon.ico" alt="">
    </div>
  </div>
</template>
