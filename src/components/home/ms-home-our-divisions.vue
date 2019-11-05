<template>
  <div class="ms-home-our-divisions">
    <div class="ms-title">
      <h3 class="section-title">Our divisisions</h3>
      <p class="section-description">
        Leveraging experience and insight to enabling peak business<br/>
        performance.
      </p>
    </div>
    <div class="ms-divisions">
      <div class="ms-division">
        <div class="ms-division-image">
          <div class="ms-divison-image-hover"></div>
          <img src="/img/home/our-division-1.jpg" alt="">
        </div>
        <div class="ms-division-name">
          CONSULTING<span class="red-dot"><i class="fa fa-square"></i></span>
        </div>
        <div class="ms-division-description">
          Delivering on a holistic, 360 strategic<br/>
          approach tailored to your enterprise<br/>
          growth agenda. 
        </div>
      </div>
      <div class="ms-division">
        <div class="ms-division-image">
          <div class="ms-divison-image-hover"></div>
          <img src="/img/home/our-division-2.jpg" alt="">
        </div>
        <div class="ms-division-name">
          COMMUNICATION<span class="red-dot"><i class="fa fa-square"></i></span>
        </div>
        <div class="ms-division-description">
          Creating platform neutral memorable<br/>
          Brand Experiences across Customer<br/>
          Journeys.
        </div>
      </div>
      <div class="ms-division">
        <div class="ms-division-image">
          <div class="ms-divison-image-hover"></div>
          <img src="/img/home/our-division-3.jpg" alt="">
        </div>
        <div class="ms-division-name">
          ASSETS<span class="red-dot"><i class="fa fa-square"></i></span>
        </div>
        <div class="ms-division-description">
          Igniting and fueling viable value<br/>
          across the stakeholder chain of a<br/>
          destination venue.
        </div>
      </div>
    </div>

    <div class="ms-read-more-wrapper">
      <button class="ms-read-more">READ MORE</button>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@import '@/assets/styles/colors.scss';

.ms-home-our-divisions {
  background-color: #f2f2f2;
  padding-top: 110px;
  padding-bottom: 110px;

  .ms-title {
    margin-left: 18vw;
    margin-bottom: 6vw;
  }

  .section-title {
    font-size: 40px;
    font-weight: bold;
    color: #000;
    margin-top: 0;
    margin-bottom: 10px;
    line-height: 59px;
  }
  .section-description {
    font-size: 18px;
    line-height: 30px;
    color: #000;
    margin-top: 0;
    margin-bottom: 60px;
  }

  .ms-divisions {
    display: flex;
    justify-content: center;

    .ms-division {
      border: 1px solid #b7b7b7;
      padding: 0 30px 50px 30px;
      margin-right: 3vw;
      color: #000;
      cursor: pointer;

      &:last-child {
        margin-right: 0;
      }

      &:hover {
        color: #fff;
        background-color: $red-light;

        .ms-division-image .ms-divison-image-hover {
          width: 100%;
          height: 330px;
          position: absolute;
          top: -45px;
          background: url('/img/add.svg'), rgba(0,0,0,0.5);
          background-repeat: no-repeat;
          background-position: center center;
          background-size: 75px 75px;
          z-index: 1;
          display: block;
        }

        .red-dot {
          color: #fff;
        } 
      }

      .ms-division-image {
        position: relative;

        .ms-divison-image-hover {
          display: none;
        }

        img {
          position: relative;
          height: 330px;
          top: -45px;
        }
      }

      .ms-division-name {
        font-size: 23px;
        line-height: 59px;
        font-weight: bold;
        margin-top: -5px;
      }

      .ms-division-description {
        font-size: 18px;
        line-height: 28px;
      }
    }
  }

  .ms-read-more-wrapper {
    margin-top: 60px;
    text-align: center;

    .ms-read-more {
      background-color: #000;
      color: #fff;
      font-size: 13px;
      padding: 24px 80px;
      border: none;
    }

    .ms-read-more:hover{
      background-color: #e82721;
    }
  }
  .red-dot {
    font-size: 10px;
    color: #e82721;
    margin-left: 4px;
  }
}
</style>
