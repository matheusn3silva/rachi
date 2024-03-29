<template>
  <h2 :class="['font-bold', 'text-2xl', 'text-center', 'mt-12', 'lg:text-[40px]']">
    {{ title }}
  </h2>
</template>

<script lang="ts" setup>
const props = defineProps({
  title: { type: String, required: true },
})
</script>
