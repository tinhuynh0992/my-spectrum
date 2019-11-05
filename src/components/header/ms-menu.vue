<template>
  <div class="ms-menu">
    <div class="ms-menu-inner">
      <!-- <div class="ms-menu-header-bg">
        <img src="@/assets/menu-bg-1.png" alt="" class="full-width"/>
      </div> -->
      <div class="ms-menu-main">
        <div class="ms-menu-top"></div>

        <div class="ms-menu-center">
          <ul class="ms-menu-primary">
            <li class="ms-menu-item"><router-link to="#">HOME</router-link></li>
            <li class="ms-menu-item"><router-link to="#">ABOUT US</router-link></li>
            <li class="ms-menu-item"><router-link to="#">ECOSYSTEM</router-link></li>
            <li class="ms-menu-item"><router-link to="#">NEWS</router-link></li>
            <li class="ms-menu-item"><router-link to="#">INSIGHTS</router-link></li>
            <li class="ms-menu-item"><router-link to="#">CONTACT US</router-link></li>
          </ul>
          <ul class="ms-menu-primary">
            <li class="ms-menu-item">
              <router-link to="#">DIVISIONS</router-link>
              <ul class="ms-menu-secondary">
                <li class="ms-menu-item"><router-link to="#">CONSULTING</router-link></li>
                <li class="ms-menu-item"><router-link to="#">COMMUNICATION</router-link></li>
                <li class="ms-menu-item"><router-link to="#">ASSETS</router-link></li>
              </ul>
            </li>
            <li class="ms-menu-item">
              <router-link to="#">BUSINESS UNITS</router-link>
              <ul class="ms-menu-secondary">
                <li class="ms-menu-item"><router-link to="#">EUROPE</router-link></li>
                <li class="ms-menu-item"><router-link to="#">AFRICA</router-link></li>
                <li class="ms-menu-item"><router-link to="#">MIDDLE EAST</router-link></li>
              </ul>
            </li>
          </ul>
        </div>

        <div class="ms-menu-bottom">
          <ul class="ms-menu-primary">
            <li class="ms-menu-item"><router-link to="#">PRIVACY POLICY</router-link></li>
            <li class="ms-menu-item"><router-link to="#">TERMS OF USE</router-link></li>
            <li class="ms-menu-item"><router-link to="#">COOKIES POLICY</router-link></li>
          </ul>
        </div>
      </div>
      <!-- <div class="ms-menu-footer-bg">
        <img src="@/assets/menu-bg-2.png" alt="" class="full-width"/>
      </div> -->
    </div>
  </div>
</template>

<style lang="scss" scoped>
@import '@/assets/styles/colors.scss';

.ms-menu {
  position: fixed;
  right: 0;
  display: flex;
  justify-content: flex-end;
  width: 100vw;
  height: 100vh;
  background-color: transparent;
  z-index: 1;

  .ms-menu-inner {
    position: relative;
    width: 50vw;
    height: 100vh;
    background-color: #ff2f29;

    .ms-menu-main {
      display: flex;
      height: 90vh;
      flex-direction: column;
      align-items: flex-start;
      justify-content: space-between;
      padding-left: 7.5vw;
      padding-top: 5vw;
      padding-bottom: 5vw;

      .ms-menu-center {
        display: flex;

        .ms-menu-item {
          list-style-type: none;
          margin-bottom: 29px;
        }

        .ms-menu-item a:hover, .ms-menu-item a:active{
          color: #fff;
        }

        a {
          font-size: 30px;
          font-weight: 900;
          text-decoration: none;
          color: #ffcbca;

          .active {
            color: #fff;
          }
        }

        .ms-menu-primary {
          .ms-menu-item {
            &:last-child {
              margin-bottom: 0;
            }
          }
        }

        .ms-menu-secondary {
          margin-top: 30px;
          margin-left: 0;
          padding-left: 20px;
          border-left: 1px solid #ffcbca;

          .ms-menu-item {
            margin-bottom: 20px;
            &:last-child {
              margin-bottom: 0;
            }

            a {
              font-size: 20px;
            }
          }
        }
      }

      .ms-menu-bottom {
        .ms-menu-primary {
          display: flex;

          .ms-menu-item {
            list-style-type: none;
            margin-right: 45px;
          }

          a:hover{
            color: #fff;
          }
        }


        a {
          font-size: 13px;
          font-weight: bold;
          line-height: 1.92;
          letter-spacing: 0.65px;
          text-decoration: none;
          color: #ffcbca;

          .active {
            color: #fff;
          }
        }
      }
    }

    .ms-menu-footer-bg {
      position: absolute;
      bottom: 0;
    }
  }
}
</style>
