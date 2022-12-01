<template>
  <header class="header">
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
      </nav>
    </div>
  </header>
</template>

<script setup>
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
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;

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
    column-gap: 56px;
  }

  &__link {
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