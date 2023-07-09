<script setup lang="ts">
import { ref } from 'vue'

const props = defineProps({
  index: {
    default: "01",
  },
  title: {
    default: "标题"
  },
  selected: {
    default: false
  }
})

const index = ref(props.index)
const title = ref(props.title)
const selected = ref(props.selected)

</script>

<template>
  <div class="mx-auto my-auto">
    <div v-if="selected" class="rounded-1/2 w-24 h-24 text-10 text-white flex justify-center items-center bg-primary">{{
      index }}</div>
    <div v-else
      class="rounded-1/2 w-24 h-24 text-10 text-primary flex justify-center items-center bg-white border border-gray-500 border-opacity-30">
      {{
        index }}</div>
    <p class="text-4">{{ title }}</p>
  </div>
</template>
