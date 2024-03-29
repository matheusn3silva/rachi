<template>
  <section
    id="home"
    :class="[
      'w-full',
      'px-6',
      'pt-44',
      'bg-[#EFF8FF]',
      'lg:h-dvh',
      'lg:flex',
      'lg:justify-around',
      'lg:px-[135px]',
      'lg:items-center',
    ]"
  >
    <div data-aos="fade-right" :class="['w-full', 'lg:max-w-[574px]']">
      <h1
        :class="[
          'font-bold',
          'leading-relaxed',
          'mb-12',
          'text-2xl',
          'sm:text-3xl',
          'md:text-5xl',
        ]"
      >
        Rachi,<br />
        é tudo que você<br />
        precisa em um só lugar.
      </h1>
      <Button
        :class="['max-w-36', 'lg:max-w-[200px]', 'text-[14px]', 'md:text-xl']"
        txt="Cadastre-se"
      />
    </div>
    <img
      data-aos="fade-left"
      data-aos-delay="500"
      :class="[
        'w-full',
        'max-w-[210px]',
        'sm:max-w-[350px]',
        'mx-auto',
        'mt-6',
        'lg:max-w-[800px]',
      ]"
      loading="lazy"
      src="../../assets/image/illustration1.svg"
      alt="Uma ilustração de um garoto de casaco, calça e gorro mexendo no notbook, sentado em cima de uma pedra ao ar livre na natureza."
    />
  </section>
</template>
