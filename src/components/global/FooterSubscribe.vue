<template>
  <nav class="subscribe">
    <input
      class="subscribe__input"
      type="email"
      placeholder="Your email..."
    >
    <button class="subscribe__button">
      Subscribe
    </button>
  </nav>
</template>

<style lang="scss" scoped>
.subscribe {
  display: flex;

  &__input {
    border: 1px solid $text-very-light;
    padding: 14px 12px;

    &::placeholder {
      color: $text-very-light;
    }

    &:focus {
      outline: none;
      border: 1px solid $brand-teal;
    }
  }

  &__button {
    font-size: 14px;
    font-family: $font-roboto;
    color: $white;
    padding: 15px 32px;
    background-color: $brand-teal;
    cursor: pointer;
    font-weight: bold;

    &:hover {
      background-color: $brand-teal--dark;
    }
  }
}
</style>