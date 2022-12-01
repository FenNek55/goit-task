<template>
  <div class="icon-card">
    <img
      class="icon-card__icon"
      :src="iconSrc"
      alt="icon"
    >
    <div class="icon-card__content">
      <h5 class="icon-card__title">
        {{ title }}
      </h5>
      <p class="icon-card__text">
        {{ text }}
      </p>
    </div>
  </div>
</template>

<script setup>
defineProps({
  iconSrc: {
    type: String,
    required: true,
  },
  title: {
    type: String,
    required: true,
  },
  text: {
    type: String,
    required: true,
  },
});
</script>

<style lang="scss" scoped>
.icon-card {
  display: flex;
  align-items: flex-start;

  &__icon {
    width: 32px;
    margin-right: 28px;
  }

  &__title {
    font-size: 14px;
    line-height: 1em;
    font-weight: normal;
    margin-bottom: 20px;
    text-transform: uppercase;
  }

  &__text {
    font-size: 15px;
    font-family: $font-roboto;
    min-height: 80px;
    color: $text-light;
    line-height: 24px;
  }
}
</style>