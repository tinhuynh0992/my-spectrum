<template>
  <div class="ms-home-business-units">
    <div class="section-text">
      <div class="section-title">
        BUSINESS<br/>
        UNITS<span class="red-dot"><i class="fa fa-square"></i></span>
      </div>
      <div class="section-description">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Morbi feugiat, felis et sagittis<br/>
        pulvinar, lacus ligula dictum libero, sit amet iaculis tellus neque sed justo. Ut vitae<br/>
        magna ac enim facilisis porta vitae eget magna. Suspendisse molestie, 
      </div>
    </div>

    <div class="section-map">
      <img src="@/assets/home-business-units-map.png" alt="" />
    </div>

    <div class="section-logo">
      <img src="@/assets/home-business-units-logo.png" alt="">
    </div>
  </div>
</template>

<style lang="scss" scoped>
.ms-home-business-units {
  background-color: transparent;
  display: flex;
  flex-direction: column;
  align-items: center;
  padding-top: 80px;
  padding-bottom: 80px;

  .section-text {
    display: flex;
    margin-bottom: 45px;

    .section-title {
      font-size: 40px;
      font-weight: bold;
      line-height: 48px;
      margin-right: 60px;
    }

    .section-description {
      font-size: 16px;
      line-height: 30px;
      color: #727272;
    }
  }

  .section-map {
    position: relative;
    z-index: 1;
  }

  .section-logo {
    margin-top: -40px;
    position: relative;
    z-index: 1;

    img {
      max-height: 150px;
    }
  }
  .red-dot {
    font-size: 10px;
    color: #e82721;
    margin-left: 4px;
  } 
}
</style>