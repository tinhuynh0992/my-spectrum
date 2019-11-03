<template>
  <div class="ms-home-slider">
    <hooper :vertical="true" style="height: 100vh" :itemsToShow="1" :centerMode="true">
      <slide>
        <div class="ms-home-slide">
          <h4 class="ms-slide-title">OUR <span class="text-red">MISSION 1</span></h4>
          <p class="ms-slide-description">
            Providing One-Stop business solutions through a<br/>
            highly connected service model, delivering actionable,<br/>
            end to end growth support to our clients.
          </p>
          <ul class="ms-slide-tags">
            <li>SOLUTIONISTS</li>
            <li><i class="fa fa-square red-dot"></i></li>
            <li>CONNECTORS</li>
            <li><i class="fa fa-square red-dot"></i></li>
            <li>VALUE CATALYSTS</li>
          </ul>
          <router-link to="#" class="ms-read-more">MORE <i class="fa fa-caret-right"></i></router-link>
        </div>
      </slide>
      <slide>
        <div class="ms-home-slide">
          <h4 class="ms-slide-title">OUR <span class="text-red">MISSION 2</span></h4>
          <p class="ms-slide-description">
            Providing One-Stop business solutions through a<br/>
            highly connected service model, delivering actionable,<br/>
            end to end growth support to our clients.
          </p>
          <ul class="ms-slide-tags">
            <li>SOLUTIONISTS</li>
            <li><i class="fa fa-square red-dot"></i></li>
            <li>CONNECTORS</li>
            <li><i class="fa fa-square red-dot"></i></li>
            <li>VALUE CATALYSTS</li>
          </ul>
          <router-link to="#" class="ms-read-more">MORE <i class="fa fa-caret-right"></i></router-link>
        </div>
      </slide>
      <slide>
        <div class="ms-home-slide">
          <h4 class="ms-slide-title">OUR <span class="text-red">MISSION 3</span></h4>
          <p class="ms-slide-description">
            Providing One-Stop business solutions through a<br/>
            highly connected service model, delivering actionable,<br/>
            end to end growth support to our clients.
          </p>
          <ul class="ms-slide-tags">
            <li>SOLUTIONISTS</li>
            <li><i class="fa fa-square red-dot"></i></li>
            <li>CONNECTORS</li>
            <li><i class="fa fa-square red-dot"></i></li>
            <li>VALUE CATALYSTS</li>
          </ul>
          <router-link to="#" class="ms-read-more">MORE <i class="fa fa-caret-right"></i></router-link>
        </div>
      </slide>
      <slide>
        <div class="ms-home-slide">
          <h4 class="ms-slide-title">OUR <span class="text-red">MISSION 4</span></h4>
          <p class="ms-slide-description">
            Providing One-Stop business solutions through a<br/>
            highly connected service model, delivering actionable,<br/>
            end to end growth support to our clients.
          </p>
          <ul class="ms-slide-tags">
            <li>SOLUTIONISTS</li>
            <li><i class="fa fa-square red-dot"></i></li>
            <li>CONNECTORS</li>
            <li><i class="fa fa-square red-dot"></i></li>
            <li>VALUE CATALYSTS</li>
          </ul>
          <router-link to="#" class="ms-read-more">MORE <i class="fa fa-caret-right"></i></router-link>
        </div>
      </slide>
    </hooper>
  </div>
</template>

<script>
import { Hooper, Slide } from 'hooper'
import 'hooper/dist/hooper.css';

export default {
  components: {
    Hooper,
    Slide
  }
}
</script>

<style lang="scss" scoped>
@import '@/assets/styles/colors.scss';

.ms-home-slider {
  height: 100vh;
  background-color: rgba(65, 65, 65, 0.58);

  .ms-home-slide {
    .ms-slide-title {
      font-size: 60px;
      font-weight: bold;
      line-height: 1.18;
      color: #fff;
      margin-top: 0;
      margin-bottom: 16px;

      .text-red {
        color: $red-dark;
      }
    }

    .ms-slide-description {
      font-size: 23px;
      font-weight: 300;
      line-height: 1.43;
      color: #fff;
    }

    .ms-slide-tags {
      display: flex;
      padding-left: 0;
      margin-bottom: 32px;

      li {
        list-style-type: none;
        margin-left: 0;
        padding-right: 20px;
        color: #fff;
        font-size: 13px;
        font-weight: bold;
        line-height: 2.31;
        letter-spacing: 1.3px;
        padding-bottom: 32px;
        border-bottom: 2px solid $red-dark;

        .red-dot {
          font-size: 9px;
          color: $red-dark;
        }

        &:last-child {
          padding-right: 0;
        }
      }

      
    }

    .ms-read-more {
      font-size: 13px;
      font-weight: bold;
      line-height: 2.31;
      color: #fff;
      text-decoration: none;
    }
  }
}
</style>
