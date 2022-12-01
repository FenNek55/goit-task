<template>
  <section class="services container">
    <div class="services__top">
      <h4 class="section-subtitle">
        We work with
      </h4>
      <h3 class="section-title">
        Amazing Services
      </h3>
    </div>
    <div class="services__grid">
      <IconCard
        v-for="service in services"
        :key="service.title"
        :icon-src="service.iconSrc"
        :title="service.title"
        :text="service.text"
      />
    </div>
  </section>
</template>

<script setup>
import IconCard from '@/components/IconCard.vue';

import aspect from '@/assets/icons/aspect.svg';
import book from '@/assets/icons/book.svg';
import computer from '@/assets/icons/computer.svg';
import house from '@/assets/icons/house.svg';
import image from '@/assets/icons/image.svg';
import timer from '@/assets/icons/timer.svg';

const services = [
  {
    title: 'Photography',
    iconSrc: timer,
    text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.',
  },
  {
    title: 'Web design',
    iconSrc: image,
    text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.',
  },
  {
    title: 'Creativity',
    iconSrc: computer,
    text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.',
  },
  {
    title: 'SEO',
    iconSrc: book,
    text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.',
  },
  {
    title: 'CSS/HTML',
    iconSrc: house,
    text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.',
  },
  {
    title: 'Digital',
    iconSrc: aspect,
    text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.',
  },
]
</script>

<style lang="scss" scoped>
.services {
  padding-top: 46px;

  &__top {
    text-align: center;
    padding-bottom: 42px;
    position: relative;
    margin-bottom: 66px;

    &::after {
      content: '';
      background-color: $brand-pink;
      width: 60px;
      height: 3px;
      position: absolute;
      left: 50%;
      bottom: 0;
      transform: translateX(-50%);
    }

  }

  &__grid {
    display: grid;
    grid-template-columns: repeat(1, 1fr);
    column-gap: 50px;
    row-gap: 58px;

    @media(min-width: $breakpoint-tablet) {
      grid-template-columns: repeat(2, 1fr);
    }

    @media(min-width: $breakpoint-desktop) {
      grid-template-columns: repeat(3, 1fr);
    }
  }
}
</style>