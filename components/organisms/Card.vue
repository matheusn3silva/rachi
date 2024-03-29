<template>
  <div
    v-if="plan == 'Prata'"
    :class="[
      'bg-[#293145]',
      'rounded-lg',
      'max-w-[370px]',
      'px-9',
      'pt-8',
      'pb-16',
      'text-white',
      'flex',
      'flex-col',
    ]"
  >
    <h4 :class="['text-center', 'font-medium', 'text-[32px]']">{{ plan }}</h4>
    <div
      :class="[
        'flex',
        'items-center',
        'justify-center',
        'bg-[#0F9AFE]',
        'w-full',
        'max-w-[164px]',
        'h-[27px]',
        'mx-auto',
        'mt-3',
        'mb-8',
        'rounded-full',
        'text-[14px]',
        'tracking-[0.2rem]',
        'font-bold',
      ]"
    >
      <p>PREFERIDO</p>
    </div>
    <h3 :class="['font-bold', 'text-center', 'text-5xl']">
      <span :class="['align-top', 'text-xl']">R$</span>{{ price
      }}<span :class="['text-[26px]']">/mês</span>
    </h3>
    <Paragraph
      :class="['mt-12', 'mb-14', 'text-[#DBDBDB]']"
      txt="Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec lacinia mi quis euismod ultrices."
    />
    <Button :class="['max-w-[230px]', 'mx-auto']" txt="Assinar" />
  </div>

  <div
    v-else
    :class="[
      'bg-[#EFF8FF]',
      'rounded-lg',
      'max-w-[370px]',
      'px-9',
      'pt-14',
      'pb-16',
    ]"
  >
    <h4 :class="['text-center', 'font-bold', 'text-2xl']">{{ plan }}</h4>
    <h3 :class="['font-bold', 'text-center', 'text-5xl', 'mt-14']">
      <span :class="['align-top', 'text-xl']">R$</span>{{ price
      }}<span :class="['text-[26px]']">/mês</span>
    </h3>
    <Paragraph
      :class="['mt-12', 'mb-14']"
      txt="Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec lacinia mi quis euismod ultrices."
    />
    <Button :class="['max-w-[230px]', 'mx-auto']" txt="Assinar" />
  </div>
</template>

<script lang="ts" setup>
const props = defineProps({
  plan: {
    type: String,
    required: true,
  },
  price: {
    type: String,
    required: true,
  },
})
</script>
