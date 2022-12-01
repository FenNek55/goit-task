<template>
  <footer class="footer container">
    <div class="footer__left">
      © 2016 MoGo free PSD template by <a href="https://www.behance.net/laaqiq">laaqiq</a> implemented by <a href="https://www.ksinteractive.pl/">Karol Stasik</a>
    </div>
    <FooterSubscribe />
  </footer>
</template>

<script setup>
import FooterSubscribe from './FooterSubscribe.vue';
</script>

<style lang="scss" scoped>
.footer {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 10px 0;
  border-top: 1px solid $text-very-light;

  &__left {
    font-size: 14px;

    a {
      color: $brand-pink;
      text-decoration: none;
    }
  }
}
</style>