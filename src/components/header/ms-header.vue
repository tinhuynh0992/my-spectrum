<template>
  <header class="ms-header">
    <div class="ms-header-layer"></div>

    <div class="ms-header-logo">
      <img src="@/assets/logo.png" alt="My Spectrum">
    </div>
    <div class="ms-menu-wrapper">
      <div class="ms-menu-button" @click="handleClickMenuButton">
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

  methods: {
    handleClickMenuButton() {
      this.menuIsActive = !this.menuIsActive

      document.body.classList.toggle("ms-menu-opened")
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
  justify-content: space-between;
  position: relative;

  .ms-header-layer {
    position: absolute;
    width: 100%;
    height: 160px;
    background-image: linear-gradient(to bottom, #000000, rgba(65, 65, 65, 0.58));
  }

  .ms-header-logo {
    display: flex;
    align-items: center;
    height: 160px;
    padding-left: 3vw;
    z-index: 1;
  }

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
        height: calc(100vh - 160px);
      }
    }
  }
}
</style>
