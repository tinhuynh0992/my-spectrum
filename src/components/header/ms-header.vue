<template>
  <div class="ms-header">
    <div class="ms-header-logo">
      <img src="@/assets/logo.png" alt="My Spectrum">
    </div>
    <div class="ms-menu-wrapper">
      <div class="ms-menu-button" @click="menuIsActive = !menuIsActive">
        <img v-if="!menuIsActive" src="@/assets/icons/menu-button.svg" alt=""/>
        <img v-else src="@/assets/icons/close-button.svg" alt=""/>
      </div>
      <ms-menu></ms-menu>
    </div>
  </div>
</template>

<script>
import msMenu from '@/components/header/ms-menu.vue'

export default {
  data() {
    return {
      menuIsActive: false
    }
  },

  components: {
    msMenu
  }
}
</script>

<style lang="scss" scoped>
@import '@/assets/styles/colors.scss';

.ms-header {
  display: flex;
  align-items: flex-start;
  justify-content: space-between;

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
}
</style>
