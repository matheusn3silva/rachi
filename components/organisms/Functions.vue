<template>
  <section id="functions" :class="['pb-24']">
    <Subtitle title="Como funciona" />
    <div
      :class="[
        'w-full',
        'mt-20',
        'flex',
        'flex-col',
        'items-center',
        'gap-8',
        'lg:flex-row',
        'lg:justify-evenly',
      ]"
    >
      <Function
        data-aos="fade-up"
        title="Crie conexões"
        text="Lorem ipsum dolor sit amet,
consecteteu."
      >
        <img
          loading="lazy"
          class="max-w-16 mx-auto"
          src="@/assets/image/user.svg"
          alt="User blue icon"
        />
      </Function>

      <Function
        data-aos="fade-up"
        data-aos-delay="500"
        title="100% gratuito"
        text="Lorem ipsum dolor sit amet,
consecteteu."
      >
        <img
          loading="lazy"
          class="max-w-16 mx-auto"
          src="@/assets/image/security.svg"
          alt="Security blue icon"
        />
      </Function>

      <Function
        data-aos="fade-up"
        data-aos-delay="1000"
        title="Compartilhamento"
        text="Lorem ipsum dolor sit amet,
consecteteu."
      >
        <img
          loading="lazy"
          class="max-w-16 mx-auto"
          src="@/assets/image/happy.svg"
          alt="Happy emoji blue icon"
        />
      </Function>
    </div>
  </section>
</template>
