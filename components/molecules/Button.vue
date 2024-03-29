<template>
  <div
    :class="[
      'bg-[#0F9AFE]',
      'text-white',
      'py-2',
      'flex',
      'justify-center',
      'items-center',
      'font-semibold',
      'rounded-full',
      'w-full',
      'cursor-pointer',
      'shadow-md',
      'shadow-[#137de080]',
    ]"
  >
    {{ txt }}
  </div>
</template>

<script lang="ts" setup>
const props = defineProps({
  txt: { type: String, required: true },
})
</script>
