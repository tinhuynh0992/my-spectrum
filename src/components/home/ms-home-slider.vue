<template>
  <div class="ms-home-slider">
    <hooper :vertical="true" style="height: 400px" :itemsToShow="1" :centerMode="true">
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
          <router-link to="#" class="ms-read-more">MORE</router-link>
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
          <router-link to="#" class="ms-read-more">MORE</router-link>
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
          <router-link to="#" class="ms-read-more">MORE</router-link>
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
          <router-link to="#" class="ms-read-more">MORE</router-link>
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
    height: 100vh;

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

      li {
        list-style-type: none;
        margin-left: 0;
        margin-right: 20px;
        color: #fff;

        &:last-child {
          margin-right: 0;
        }
      }
    }

    .ms-read-more {
      color: #fff;
    }
  }
}
</style>
