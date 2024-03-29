<template>
  <div :class="['max-w-[210px]', 'flex', 'flex-col', 'justify-center']">
    <slot />
    <h4
      :class="['mt-8', 'text-center', 'font-bold', 'text-base', 'lg:text-xl']"
    >
      {{ title }}
    </h4>
    <Paragraph :txt="text" :class="['mt-4']" />
  </div>
</template>

<script lang="ts" setup>
const props = defineProps({
  title: { type: String, required: true },
  text: { type: String, required: true },
})
</script>
