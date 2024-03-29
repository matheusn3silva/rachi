<template>
  <nav>
    <button id="btn-mobile" @click="toggleMenu" :class="['md:hidden']">
      <span
        id="hamburger"
        :class="['w-full', 'border-t-[3px]', 'border-solid', 'border-black']"
      ></span>
    </button>
    <ul
      id="menu"
      :class="[
        'w-full',
        'gap-16',
        'absolute',
        'top-20',
        'left-0',
        'bg-white',
        'md:p-0',
        'md:flex',
        'md:items-center',
        'md:static',
        'md:visible',
        'z-[1000]',
      ]"
    >
      <li>
        <a
          @click="toggleMenu"
          :class="[
            'block',
            'py-6',
            'px-8',
            'hover:bg-slate-200',
            'md:hover:bg-transparent',
            'md:p-2',
          ]"
          href="#functions"
          >Funcionalidades</a
        >
      </li>
      <li>
        <a
          @click="toggleMenu"
          :class="[
            'block',
            'py-6',
            'px-8',
            'hover:bg-slate-200',
            'md:hover:bg-transparent',
            'md:p-2',
          ]"
          href="#app"
          >App</a
        >
      </li>
      <li>
        <a
          @click="toggleMenu"
          :class="[
            'block',
            'py-6',
            'px-8',
            'hover:bg-slate-200',
            'md:hover:bg-transparent',
            'md:p-2',
          ]"
          href="#plans"
          >Planos</a
        >
      </li>
      <li>
        <a
          @click="toggleMenu"
          :class="[
            'block',
            'py-6',
            'px-8',
            'hover:bg-slate-200',
            'md:hover:bg-transparent',
            'md:p-2',
          ]"
          href="#contact"
          >Contato</a
        >
      </li>
    </ul>
  </nav>
</template>

<script lang="ts" setup>
const toggleMenu = () => {
  const nav = document.querySelector('nav') as HTMLElement
  nav.classList.toggle('active-menu')
}
</script>

<style scoped>
a {
  color: #6e7275;
}

a:hover {
  color: #0f9afe;
}

@media (max-width: 768px) {
  #menu {
    transition: 0.6s;
    height: 0;
    visibility: hidden;
    overflow-y: hidden;
  }

  nav.active-menu #menu {
    height: 288px;
    visibility: visible;
  }

  #btn-mobile {
    width: 30px;
    height: 30px;
    position: relative;
  }

  #hamburger {
    display: block;
  }

  #hamburger::after,
  #hamburger::before {
    content: '';
    display: block;
    width: 100%;
    height: 2px;
    margin-top: 7px;
    background: currentColor;
  }

  #hamburger::after {
    width: 50%;
    right: 0;
    position: absolute;
  }
}
</style>
