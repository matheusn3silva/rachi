<template>
  <section
    id="contact"
    :class="[
      'bg-center',
      'bg-no-repeat',
      'relative',
      'px-6',
      'pt-[50px]',
      'pb-24',
    ]"
  >
    <div
      :class="[
        'w-full',
        'h-full',
        'absolute',
        'inset-0',
        'backdrop-brightness-[0.50]',
        'backdrop-blur',
        'z-[1]',
      ]"
    ></div>
    <Subtitle
      data-aos="zoom-in"
      :class="['text-white', 'mb-4', 'relative', 'z-10']"
      title="Contato"
    />
    <Paragraph
      data-aos="zoom-in"
      :class="[
        'max-w-80',
        'mx-auto',
        'text-[#DBDBDB]',
        'relative',
        'z-10',
        'lg:max-w-[520px]',
      ]"
      txt="Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec lacinia mi quis euismod ultrices."
    />

    <EmailForm data-aos="zoom-in" :class="['relative', 'z-10']" />
  </section>
</template>

<style>
#contact {
  background-image: url('../../assets/image/computer.png');
}
</style>
