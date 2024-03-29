<template>
  <section id="plans" :class="['pb-32', 'px-6']">
    <Subtitle data-aos="fade-down" title="Nossos Planos" />
    <Paragraph
      data-aos="fade-down"
      :class="[
        'max-w-80',
        'mx-auto',
        'mt-4',
        'mb-24',
        'text-center',
        'lg:max-w-[550px]',
        'lg:text-[18px]',
      ]"
      txt="Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec lacinia mi quis euismod ultrices."
    />
    <div
      :class="[
        'w-full',
        'flex',
        'flex-col',
        'items-center',
        'justify-center',
        'gap-8',
        'lg:flex-row',
      ]"
    >
      <Card data-aos="fade-up" plan="Bronze" price="28" />
      <Card data-aos="fade-up" data-aos-delay="600" plan="Prata" price="57" />
      <Card data-aos="fade-up" data-aos-delay="300" plan="Ouro" price="94" />
    </div>
  </section>
</template>
