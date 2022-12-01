<template>
  <section class="about container">
    <div class="about__top">
      <h4 class="section-subtitle">
        Who we are
      </h4>
      <h3 class="section-title">
        Meet our team
      </h3>
    </div>
    <p class="about__description">
      Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
    </p>
    <div class="about__grid">
      <section class="about__entry">
        <AboutCard
          class="about__card"
          :img-src="matthew"
        />
        <h5 class="about__name">
          Matthew Dix
        </h5>
        <p class="about__position">
          Graphic Designer
        </p>
      </section>
      <section class="about__entry">
        <AboutCard
          class="about__card"
          :img-src="christopher"
        />
        <h5 class="about__name">
          Christopher Campbell
        </h5>
        <p class="about__position">
          Branding/UX design
        </p>
      </section>
      <section class="about__entry">
        <AboutCard
          class="about__card"
          :img-src="michael"
        />
        <h5 class="about__name">
          Michael Fertig
        </h5>
        <p class="about__position">
          Developer
        </p>
      </section>
    </div>
  </section>
</template>

<script setup>
import AboutCard from '@/components/AboutCard.vue';
import matthew from '@/assets/images/matthew.png';
import christopher from '@/assets/images/christopher.png';
import michael from '@/assets/images/michael.png';
</script>

<style lang="scss" scoped>
.about {
  padding-top: 50px;
  margin-bottom: 84px;

  &__top {
    text-align: center;
    padding-bottom: 42px;
    position: relative;
    margin-bottom: 46px;

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

  &__description {
    max-width: 960px;
    text-align: center;
    margin: 0 auto;
    font-size: 15px;
    color: $text-light;
    margin-bottom: 90px;
  }

  &__grid {
    display: grid;
    grid-template-columns: repeat(1, 1fr);
    column-gap: 30px;
    row-gap: 78px;

    @media(min-width: $breakpoint-tablet) {
      grid-template-columns: repeat(2, 1fr);
    }

    @media(min-width: $breakpoint-desktop) {
      grid-template-columns: repeat(3, 1fr);
    }
  }

  &__card {
    margin-bottom: 28px;
  }

  &__name {
    font-size: 14px;
    margin-bottom: 16px;
    text-align: center;
    font-weight: 400;
  }

  &__position {
    font-size: 15px;
    color: $text-light;
    font-weight: light;
    font-size: italic;
    text-align: center;
    font-family: $font-roboto;
  }
}
</style>