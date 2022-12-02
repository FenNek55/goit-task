<template>
  <section class="hero">
    <div class="container hero__content">
      <h2 class="hero__subtitle">
        Creative Template
      </h2>
      <h1 class="hero__title">
        Welcome<br>
        to MoGo
      </h1>
      <button class="hero__cta">
        Leran More
      </button>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.hero {
  padding: 236px 0;
  background-image: url('@/assets/images/hero-bg.png');
  background-image: linear-gradient(to bottom, #{$brand-pink}E6, #{$brand-yellow}E6), url('@/assets/images/hero-bg.png');
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
  line-height: 1em;

  &__content {
    margin: 0 auto;
    width: fit-content;
    text-align: center;
  }

  &__subtitle {
    font-family: $font-kaushan;
    font-size: calc(72px * 0.3);
    margin-bottom: 20px;
    color: white;

    @media (min-width: $breakpoint-tablet) {
      font-size: calc(72px * 0.6);
      margin-bottom: 60px;
    }

    @media (min-width: $breakpoint-desktop) {
      font-size: 72px;
    }
  }

  &__title {
    font-size: calc(150px * 0.4);
    margin-bottom: 124px;
    color: white;

    @media (min-width: $breakpoint-tablet) {
      font-size: calc(150px * 0.75);
      line-height: calc(140px * 0.75);
    }

    @media (min-width: $breakpoint-desktop) {
      font-size: 150px;
      line-height: 140px;;
    }
  }

  &__cta {
    color: white;
    padding: 15px 32px;
    border: 4px solid $white;
    background-color: transparent;
    font-weight: bold;
    font-size: 14px;
    text-transform: uppercase;
    cursor: pointer;
  }
}
</style>