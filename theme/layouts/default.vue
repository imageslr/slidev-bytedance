<template>
  <div class="slidev-layout default">
    <img src="/images/logo-2.png" class="logo" />
    <slot />
    <div class="slide-number">
      <SlideCurrentNo /> /
      <SlidesTotal />
    </div>
  </div>
</template>
