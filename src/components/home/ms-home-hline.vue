<template>
  <div class="ms-home-hline">
    <div class="ms-home-hline-logo">
      <img src="@/assets/home-hline-logo.svg" alt="">
    </div>

    <div class="ms-menu-wrapper">
      <div class="ms-menu-button" @click="menuIsActive = !menuIsActive">
        <img v-if="!menuIsActive" src="@/assets/icons/menu-button.svg" alt=""/>
        <img v-else src="@/assets/icons/close-button.svg" alt=""/>
      </div>
    </div>

    <ms-menu v-if="menuIsActive"></ms-menu>
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

.ms-home-hline {
  height: 80px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #000;

  .ms-home-hline-logo {
    padding-left: 3vw;
  }

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
  .ms-home-hline-logo img{
    width: 220px;
    height: 40px;
    object-fit: contain;
  }
  .ms-home-hline-logo{
    display: flex;
    align-items: center;
    margin-left: 4vw;
  }
}
</style>
