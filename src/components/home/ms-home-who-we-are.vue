<template>
  <div class="ms-home-who-we-are" id="home-who-we-are">
    <div class="ms-row">
      <div class="ms-text">
        <h4 class="ms-subtitle">WHO WE ARE</h4>
        <h3 class="ms-title">SOLUTIONISTS &<br/>CONNECTORS<i class="fa fa-square"></i></h3>
        <p class="ms-description">
          Connecting the right strategy, tools, and networks to our clients'
          needs, providing a one stop solution via hands-on engagements through
          a highly connected service model, delivering end-to-end growth
          support, across the different phases of our clients' growth journey.
        </p>
      </div>
      <div class="ms-image style-1">
        <img src="/img/home/who-we-are-1.png" alt="Solutionists & Connectors" />
      </div>
    </div>

    <div class="ms-row">
      <div class="ms-image style-2">
        <img src="/img/home/who-we-are-2.png" alt="Value Catalyst" />
      </div>
      <div class="ms-text">
        <h4 class="ms-subtitle">WHO WE ARE</h4>
        <h3 class="ms-title">VALUE CATALYSTS<i class="fa fa-square"></i></h3>
        <p class="ms-description">
          Our business model is a Partner based model which drives Growth
          Strategy, Organizational Transformation and Business Management
          Initiatives while tapping into necessary in-depth discipline and
          industry experts as required via our local, regional and
          international Affiliate Partner network.
        </p>

        <div class="ms-read-more-wrapper">
          <button class="ms-read-more">READ MORE</button>
        </div>
      </div>
    </div>

  </div>
</template>

<style lang="scss" scoped>
@import '@/assets/styles/colors.scss';

.ms-home-who-we-are {
  .ms-row {
    width: 75vw;
    margin: 0 auto;
    display: flex;

    &:first-child {
      margin-bottom: 84px;
    }

    .ms-image {
      background-color: #fff;
      position: relative;

      &.style-1 {
        box-shadow: 30px -30px 30px 0 rgba(0, 0, 0, 0.05);
        margin-top: 6.3vw;

        img {
          position: relative;
          top: 24px;
          right: 24px;
        }
      }

      &.style-2 {
        box-shadow: -30px 30px 30px 0 rgba(0, 0, 0, 0.05);
        margin-bottom: 5.5vw;

        img {
          position: relative;
          bottom: 24px;
          left: 24px;
        }
      }
    }

    .ms-text {
      padding: 4vw 5.5vw 4vw 4vw;
      .ms-subtitle {
        font-size: 14px;
        font-weight: bold;
        color: #000;
        margin-bottom: 15px;
      }

      .ms-title {
        font-size: 40px;
        font-weight: bold;
        line-height: 1.23;
        color: #000;
        margin-top: 0;
        margin-bottom: 25px;

        .red-dot {
          color: $red-dark;
        }
      }

      .ms-description {
        font-size: 16px;
        color: #000;
        margin-bottom: 0;
      }

      .ms-read-more-wrapper {
        margin-top: 60px;

        .ms-read-more {
          background-color: #000;
          color: #fff;
          font-size: 13px;
          padding: 24px 80px;
          border: none;
        }
      }
    }
    .ms-title i{
      font-size: 10px;
      margin-left: 3px;
      color: #e82721;
    }
  }
}
</style>