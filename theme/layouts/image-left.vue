<script setup lang="ts">
import { computed } from 'vue'
import { handleBackground } from '../layoutHelper'

const props = defineProps({
  image: {
    type: String,
  },
  class: {
    type: String,
  },
})

const style = computed(() => handleBackground(props.image))
</script>

<template>
  <div class="grid grid-cols-2 w-full h-full auto-rows-fr">
    <div class="w-full -full" :style="style" />
    <div class="slidev-layout default" :class="props.class">
      <img src="/images/logo-2.png" class="logo"/>
      <slot />
    </div>
  </div>
</template>