<template>
  <p :class="['text-[#6E7275]', 'text-[14px]', 'lg:text-base', 'text-center']">
    {{ txt }}
  </p>
</template>

<script lang="ts" setup>
const props = defineProps({
  txt: { type: String, required: true },
})
</script>
