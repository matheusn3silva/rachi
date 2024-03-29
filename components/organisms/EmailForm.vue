<template>
  <form :class="['mt-24']" @submit.prevent>
    <div
      :class="[
        'w-full',
        'max-w-[500px]',
        'mx-auto',
        'flex',
        'flex-col',
        'gap-9',
        'justify-between',
        'lg:flex-row',
      ]"
    >
      <input
        :class="[
          'bg-transparent',
          'w-full',
          'block',
          'border-b-[1px]',
          'border-white',
          'outline-none',
          'py-2',
          'font-semibold',
          'text-white',
          'placeholder:text-white',
          'placeholder:text-[18px]',
          'placeholder:font-semibold',
          'lg:w-[300px]',
        ]"
        type="email"
        name="email"
        placeholder="Seu melhor e-mail"
      />
      <button :class="['w-full', 'lg:w-[118px]']" type="submit">
        <Button :class="['w-full']" txt="Enviar" />
      </button>
    </div>
  </form>
</template>
