<template>
  <div class="container">
    <footer class="footer">
      <div class="footer__left">
        © 2016 MoGo free PSD template by <a href="https://www.behance.net/laaqiq">laaqiq</a> implemented by <a href="https://www.ksinteractive.pl/">Karol Stasik</a>
      </div>
      <FooterSubscribe />
    </footer>
  </div>
</template>

<script setup>
import FooterSubscribe from './FooterSubscribe.vue';
</script>

<style lang="scss" scoped>
.footer {
  display: flex;
  flex-direction: column;
  padding: 10px 0;
  border-top: 1px solid $text-very-light;

  @media (min-width: $breakpoint-tablet) {
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
  }

  &__left {
    font-size: 14px;
    margin-bottom: 56px;

    @media(min-width: $breakpoint-tablet) {
      margin-bottom: 0;
    }

    a {
      color: $brand-pink;
      text-decoration: none;
    }
  }
}
</style>