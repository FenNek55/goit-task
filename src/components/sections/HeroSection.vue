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
  color: white;

  &__content {
    margin: 0 auto;
    width: fit-content;
    text-align: center;
  }

  &__subtitle {
    font-family: $font-kaushan;
    font-size: 76px;
    margin-bottom: 60px;
  }

  &__title {
    font-size: 150px;
    line-height: 140px;
    margin-bottom: 124px;
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