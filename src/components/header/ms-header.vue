<template>
  <header class="ms-header">
    <div class="ms-header-logo">
      <img src="@/assets/logo.png" alt="My Spectrum">
    </div>
    <div class="ms-menu-wrapper">
      <div class="ms-menu-button" @click="menuIsActive = !menuIsActive">
        <img v-if="!menuIsActive" src="@/assets/icons/menu-button.svg" alt=""/>
        <img v-else src="@/assets/icons/close-button.svg" alt=""/>
      </div>

      <ms-lang-switcher></ms-lang-switcher>

      <div class="ms-menu-logo-wrapper" v-if="menuIsActive">
        <img src="@/assets/menu-logo.png" alt="My Spectrum">
      </div>
    </div>

    <ms-menu v-if="menuIsActive"></ms-menu>
  </header>
</template>

<script>
import msMenu from '@/components/header/ms-menu.vue'
import msLangSwitcher from '@/components/header/ms-lang-switcher.vue'

export default {
  data() {
    return {
      menuIsActive: false
    }
  },

  components: {
    msMenu,
    msLangSwitcher
  }
}
</script>

<style lang="scss" scoped>
@import '@/assets/styles/colors.scss';

.ms-header {
  display: flex;
  align-items: flex-start;
  justify-content: space-between;
  position: relative;
  background-image: linear-gradient(to bottom, #000000, rgba(65, 65, 65, 0.58));

  .ms-menu-wrapper {
    display: flex;
    flex-direction: column;
    align-items: flex-end;
    z-index: 10;

    .ms-menu-button {
      width: 80px;
      height: 80px;
      display: flex;
      justify-content: center;
      align-items: center;
      background-color: $red-dark;
      cursor: pointer;

      img {
        width: 20px;
        height: 20px;
      }
    }

    .ms-menu-logo-wrapper {
      img {
        height: calc(100vh - 80px);
      }
    }
  }
}
</style>
