<template>
  <section
    id="app"
    :class="[
      'w-full',
      'bg-[#EFF8FF]',
      'px-6',
      'py-9',
      'lg:flex',
      'lg:justify-evenly',
      'lg:items-center',
    ]"
  >
    <div data-aos="flip-right" data-aos-delay="500">
      <Subtitle
        :class="['text-2xl', 'lg:text-start', 'lg:text-3xl']"
        title="Baixe nosso app para desfrutar mais!"
      />
      <Paragraph
        :class="['mx-auto', 'max-w-[420px]', 'mt-6', 'mb-8', 'lg:text-start']"
        txt="Amet in elementum nulla scelerisque dui, egestas at. Elit consectetur turpis elementum amet vitae et etiam nec. Varius volutpat hac adipiscing tincidunt pretium."
      />
      <span
        :class="[
          'w-full',
          'mx-auto',
          'max-w-[300px]',
          'flex',
          'gap-6',
          'justify-center',
        ]"
      >
        <img
          :class="['max-w-32', 'cursor-pointer', 'md:max-w-full']"
          loading="lazy"
          src="@/assets/image/google-play.svg"
          alt="Botão de download do app no aplicativo da google play, com fundo preto e texto e imagens branco"
        />
        <img
          :class="['max-w-32', 'cursor-pointer', 'md:max-w-full']"
          loading="lazy"
          src="@/assets/image/app-store.svg"
          alt="Botão de download do app no aplicativo da app store, com fundo preto e texto e imagens branco"
        />
      </span>
    </div>
    <img
      data-aos="zoom-out"
      data-aos-delay="500"
      :class="['hidden', 'max-w-[400px]', 'lg:block ']"
      loading="lazy"
      src="@/assets/image/illustration2.svg"
      alt=""
    />
  </section>
</template>

<script lang="ts" setup></script>
