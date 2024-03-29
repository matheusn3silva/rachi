<template>
  <header
    :class="[
      'bg-white',
      'w-full',
      'h-20',
      'p-6',
      'flex',
      'justify-between',
      'items-center',
      'fixed',
      'lg:px-32',
      'z-50',
    ]"
  >
    <a href="#home" class="max-w-[72px]">
      <Logo />
    </a>
    <Navigation />
  </header>
</template>
