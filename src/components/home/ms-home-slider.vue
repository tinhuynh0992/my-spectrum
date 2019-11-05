<template>
  <div class="ms-home-slider">
    <hooper :vertical="true" style="height: 100vh" :itemsToShow="1" :centerMode="true" :wheelControl="false">
      <slide>
        <div class="ms-home-slide" :style="{
          backgroundImage: 'url(\'/img/home/home-slider-bg-1.jpg\')',
          backgroundRepeat: 'no-repeat',
          backgroundPosition: 'center center',
          backgroundSize: 'cover'
        }">
          <div class="ms-home-slide-layer"></div>

          <div class="ms-home-slide-content">
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
            <router-link to="#" class="ms-read-more">MORE<i class="fa fa-caret-right"></i></router-link>
          </div>
        </div>
      </slide>
      <slide>
        <div class="ms-home-slide" :style="{
          background: 'url(\'/img/home/home-slider-bg-2.jpg\')',
          backgroundRepeat: 'no-repeat',
          backgroundPosition: 'center center',
          backgroundSize: 'cover'
        }">
          <div class="ms-home-slide-layer"></div>

          <div class="ms-home-slide-content">
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
            <router-link to="#" class="ms-read-more">MORE<i class="fa fa-caret-right"></i></router-link>
          </div>
        </div>
      </slide>
      <slide>
        <div class="ms-home-slide" :style="{
          background: 'url(\'/img/home/home-slider-bg-3.jpg\')',
          backgroundRepeat: 'no-repeat',
          backgroundPosition: 'center center',
          backgroundSize: 'cover'
        }">
          <div class="ms-home-slide-layer"></div>

          <div class="ms-home-slide-content">
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
            <router-link to="#" class="ms-read-more">MORE<i class="fa fa-caret-right"></i></router-link>
          </div>
        </div>
      </slide>
      <slide>
        <div class="ms-home-slide" :style="{
          background: 'url(\'/img/home/home-slider-bg-4.jpg\')',
          backgroundRepeat: 'no-repeat',
          backgroundPosition: 'center center',
          backgroundSize: 'cover'
        }">
          <div class="ms-home-slide-layer"></div>

          <div class="ms-home-slide-content">
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
            <router-link to="#" class="ms-read-more">MORE<i class="fa fa-caret-right"></i></router-link>
          </div>
        </div>
      </slide>

      <pagination slot="hooper-addons"></pagination>
    </hooper>

    <div class="ms-slider-bottom-left">
      <img src="@/assets/home-slider-map.png" alt="" />
    </div>

    <div class="ms-slider-bottom-right">
      <hr class="ms-slider-bottom-right-line">
      <span @click="handleScrollDown">SCROLL</span>
    </div>
  </div>
</template>

<script>
import { Hooper, Slide, Pagination } from 'hooper'
import 'hooper/dist/hooper.css';

export default {
  components: {
    Hooper,
    Slide,
    Pagination
  },

  methods: {
    handleScrollDown() {
      document.getElementById("home-who-we-are").scrollIntoView({behavior: "smooth"});
    }
  }
}
</script>

<style lang="scss" scoped>
@import '@/assets/styles/colors.scss';

.ms-home-slider {
  position: relative;
  height: 100vh;
  background-color: rgba(65, 65, 65, 0.58);
  overflow: hidden;

  .ms-home-slide {
    height: 100vh;
    position: relative;
    display: flex;
    flex-direction: column;
    justify-content: center;

    .ms-home-slide-layer {
      position: absolute;
      width: 100%;
      top: 160px;
      height: calc(100vh - 160px);
      background-color: rgba(65, 65, 65, 0.58);
      z-index: 1;
    }

    .ms-home-slide-content {
      padding-left: 15vw;
      z-index: 1;
    }

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

      .fa {
        margin-left: 10px;
      }
    }
  }

  .ms-slider-bottom-left {
    position: absolute;
    bottom: -100px;
    left: -50px;
  }

  .ms-slider-bottom-right {
    position: absolute;
    bottom: 0;
    right: 0;
    display: flex;
    align-items: center;
    cursor: pointer;
    transform: rotate(-90deg);
    -moz-transform: rotate(-90deg);
    -webkit-transform: rotate(-90deg);
    -o-transform: rotate(-90deg);
    margin-right: 30px;
    padding-top: 195px;

    .ms-slider-bottom-right-line {
      width: 125px;
      margin-right: 30px;
    }

    span {
      font-size: 10px;
      font-weight: bold;
      line-height: 1.1;
      letter-spacing: 3px;
      text-align: left;
      color: #fff;
      text-decoration: none;
    }
  }
}
</style>

<style lang="scss">
@import '@/assets/styles/colors.scss';

.hooper {
  .hooper-pagination.is-vertical {
    top: 50vh;
    padding-right: 30px;

    .hooper-indicator {
      width: 7px;
      height: 7px;
      margin-bottom: 30px;

      &:hover {
        background-color: $red-dark;
      }

      &.is-active {
        background-color: $red-dark;
      }
    }

  }
}
</style>
