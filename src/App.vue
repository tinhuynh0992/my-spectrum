<template>
  <div id="app">
    <ms-header/>
    <div class="main-wrapper">
      <router-view/>
    </div>
    <ms-footer/>
  </div>
</template>

<script>
import msHeader from '@/components/header/ms-header'
import msFooter from '@/components/footer/ms-footer'

export default {
  components: {
    msHeader,
    msFooter
  }
}
</script>

<style lang="scss">
#app {
  font-family: 'Roboto', sans-serif;
}
</style>
