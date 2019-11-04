<template>
  <div id="app">
    <div class="main-wrapper">
      <router-view/>
    </div>
    <ms-footer/>
  </div>
</template>

<script>
import msFooter from '@/components/footer/ms-footer'

export default {
  components: {
    msFooter
  }
}
</script>

<style lang="scss">
body {
  margin: 0;
  padding: 0;

  &.ms-menu-opened {
    overflow-y: hidden;
  }
}
#app {
  font-family: 'Roboto', sans-serif;

  .full-width {
    width: 100%;
  }
}
</style>
