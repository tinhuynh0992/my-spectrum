<template>
  <div class="ms-statistic">
    <div class="ms-box">
      <div class="ms-text">
        <h4>100+</h4>
        <p>BRAND EXPERIENCE</p>
        <img src="@/assets/icons/page-statistic/icon-statistic.png" alt="Icon Statistic">
      </div>
      <div class="ms-text">
        <h4>20+</h4>
        <p>COUNTRY EXPERIENCE</p>
        <img src="@/assets/icons/page-statistic/icon-statistic.png" alt="Icon Statistic">
      </div>
      <div class="ms-text">
        <h4>200+</h4>
        <p>PROJECTS</p>
        <img src="@/assets/icons/page-statistic/icon-statistic.png" alt="Icon Statistic">
      </div>
      <div class="ms-text">
        <h4>95%</h4>
        <p>SOMETHING ELSE</p>
        <img src="@/assets/icons/page-statistic/icon-statistic.png" alt="Icon Statistic">
      </div>
      <div class="ms-text">
        <h4>450+</h4>
        <p>EMPLOVESS</p>
        <img src="@/assets/icons/page-statistic/icon-statistic.png" alt="Icon Statistic">
      </div>
    </div>

    <div class="ms-particle-wrapper">
      <ms-particle
        width="30vw"
        height="30vw"
        link-color="#e82721"
        :number-particles="20"
      ></ms-particle>
    </div>
  </div>
</template>

<script>
import msParticle from '@/components/ms-particle.vue'

export default {
  components: {
    msParticle
  }
}
</script>

<style lang="scss" scoped>
.ms-statistic {
  margin-top: 166px;
  background-color: transparent;
  position: relative;

  h4 {
    font-size: 43px;
    font-weight: bold;
    letter-spacing: -0.86px;
    text-align: center;
    color: #fff;
    margin: 0;
  }
  .ms-box {
    border-top: 3px solid #e82721;
    width: 74.5vw;
    height: 12.5vw;
    box-shadow: 0 14px 26px 0 rgba(0, 0, 0, 0.04);
    background-color: #000000;
    display: flex;
    margin-left: auto;
    margin-right: auto;
    justify-content: center;
    align-items: center;
    position: relative;
    margin-bottom: -35px;
  }
  .ms-text {
    font-size: 14px;
    font-weight: bold;
    line-height: 1.14;
    letter-spacing: 0.56px;
    text-align: center;
    color: #fff;
    margin-right: 3vw;
    margin-left: 3vw;
  }

  .ms-particle-wrapper {
    position: absolute;
    right: 0;
    bottom: 0;
    z-index: -1;
  }
}
</style>
