<template>
  <header
    class="header"
    :class="{
      'header--sticky': isSticky,
    }"
  >
    <div class="container header__container">
      <a
        href="/"
        class="header__logo"
      >
        MoGo
      </a>
      <nav class="header__links">
        <a
          v-for="link in links"
          :key="link.name"
          :href="link.path"
          class="header__link"
        >{{ link.name }}</a>
        <a
          href="/"
          class="header__link--with-icon"
        ><SearchIcon class="header__icon" /></a>
        <a
          href="/"
          class="header__link--with-icon"
        ><CartIcon class="header__icon" /></a>
      </nav>
    </div>
  </header>
</template>

<script setup>
import CartIcon from '@/components/icons/CartIcon.vue';
import SearchIcon from '@/components/icons/SearchIcon.vue';
import { onMounted, ref } from 'vue';

const isSticky = ref(false);

onMounted(() => {
  window.addEventListener('scroll', () => {
    if (window.scrollY > 0) {
      isSticky.value = true;
    } else {
      isSticky.value = false;
    }
  });
})

const links = [
  {
    name: 'About',
    path: '/',
  },
  {
    name: 'Service',
    path: '/service',
  },
  {
    name: 'Work',
    path: '/services',
  },
  {
    name: 'Blog',
    path: '/blog',
  },
  {
    name: 'Contact',
    path: '/contact',
  },
];
</script>

<style lang="scss" scoped>
.header {
  z-index: 100;
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  transition: background-color 0.2s;

  &--sticky {
    background-color: $brand-pink;
  }

  &__container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 26px 0; 
    color: $white;
  }
  
  &__logo {
    font-weight: bold;
    font-size: 30px;
    text-decoration: none;
    color: white;
    transition: color 0.6s;

    &:hover {
      color: $brand-yellow;
    }
  }

  &__links {
    display: flex;
    align-items: center;
  }

  &__link {
    margin-right: 56px;
    position: relative;
    font-size: 14px;
    font-weight: 400;
    text-decoration: none;
    color: $white;
    text-transform: uppercase;
    transition: color 0.6s;

    &--active {
      color: $brand-yellow;
    }

    &--with-icon {
      width: 20px;
      height: 20px;
      margin-right: 42px;
    }

    &:hover {
      color: $brand-yellow;
    }

    &::after {
      content: '';
      position: absolute;
      bottom: -12px;
      left: 50%;
      width: 0%;
      height: 2px;
      background-color: $brand-yellow;
      transition: transform 0.6s, width 0.6s;
      transform: translateX(-50%);
    }

    &:hover::after {
      width: 100%;
    }
  }
}
</style>