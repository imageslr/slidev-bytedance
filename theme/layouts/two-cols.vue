<!--
  Usage:

```md
---
layout: two-cols
---

# Left

This shows on the left

::right::

# Right

This shows on the right
```

-->

<script setup lang="ts">
const props = defineProps({
  class: {
    type: String,
  },
  layoutClass: {
    type: String,
  },
})
</script>

<template>
  <div class="slidev-layout two-columns w-full h-full grid grid-cols-2" :class="props.layoutClass">
    <img src="/images/logo-2.png" class="logo" />
    <div class="col-left" :class="props.class">
      <slot />
    </div>
    <div class="col-right" :class="props.class">
      <slot name="right" />
    </div>

    <div class="slide-number">
      <SlideCurrentNo /> /
      <SlidesTotal />
    </div>
  </div>
</template>