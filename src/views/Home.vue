<template>
  <div class="home-page">
    <div class="ms-nav-slider">
      <ms-header/>
      <ms-home-slider></ms-home-slider>
    </div>

    <ms-home-who-we-are></ms-home-who-we-are>
    <ms-home-our-divisions></ms-home-our-divisions>
    <ms-home-hline></ms-home-hline>
    <ms-home-business-units></ms-home-business-units>
    <ms-home-client-portfolio></ms-home-client-portfolio>
    <ms-home-statistic></ms-home-statistic>
    <ms-home-latest-news></ms-home-latest-news>
  </div>
</template>

<script>
import msHeader from '@/components/header/ms-header'
import msHomeSlider from '@/components/home/ms-home-slider.vue'
import msHomeWhoWeAre from '@/components/home/ms-home-who-we-are.vue'
import msHomeOurDivisions from '@/components/home/ms-home-our-divisions.vue'
import msHomeHline from '@/components/home/ms-home-hline.vue'
import msHomeBusinessUnits from '@/components/home/ms-home-business-units.vue'
import msHomeClientPortfolio from '@/components/home/ms-home-client-portfolio.vue'
import msHomeStatistic from '@/components/home/ms-home-statistic.vue'
import msHomeLatestNews from '@/components/home/ms-home-latest-news.vue'

export default {
  name: 'home',
  components: {
    msHeader,
    msHomeSlider,
    msHomeWhoWeAre,
    msHomeOurDivisions,
    msHomeHline,
    msHomeBusinessUnits,
    msHomeClientPortfolio,
    msHomeStatistic,
    msHomeLatestNews
  }
}
</script>

<style lang="scss" scoped>
.ms-nav-slider {
  background: url('/img/home/home-slider-bg.jpg');
  background-repeat: no-repeat;
  background-position: center center;
}
</style>