<template>
  <div class="ms-latest-new">
    <div class="ms-background">
      <img src="@/assets/icons/page-last-new/intersection-15.png" alt="anc">
      <img src="@/assets/icons/page-last-new/intersection-16.png" alt="aanc">
    </div>
    <div class="ms-title">
      <h1>LATEST NEWS & INSIGHTS<i class="fa fa-square"></i></h1>
    </div>
    <div class="ms-icon">
      <a href="#"><img src="@/assets/icons/arrow-icon-2.svg" alt="arrow icon"></a>
      <a href="#"><img src="@/assets/icons/arrow-icon-1.svg" alt="arrow icon"></a>
    </div>
    <div class="ms-posts-wrapper">
      <div class="ms-posts">
        <div class="ms-post">
          <div class="ms-post-image">
            <img src="/img/home/last-new-1.jpg" alt="Last new post 1">
            <span class="badge">NEWS</span>
          </div>
          <div class="ms-post-text">
            <p class="ms-post-date">04/03/2019</p>
            <h4 class="ms-post-title">Creating value beyond the deal</h4>
            <p class="ms-post-description">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. 
              Morbi feugiat, felis et sagittis pulvinar …
            </p>
          </div>

          <div class="ms-post-layer">
            <div class="ms-post-tags">
              <span class="badge">NEWS</span>
            </div>
            <p class="ms-post-date">04/03/2019</p>
            <h4 class="ms-post-title">Creating value beyond the deal</h4>
            <p class="ms-post-description">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. 
              Morbi feugiat, felis et sagittis pulvinar …
            </p>
          </div>
        </div>
        <div class="ms-post">
          <div class="ms-post-image">
            <img src="/img/home/last-new-2.jpg" alt="Last new post 1">
            <span class="badge">NEWS</span>
          </div>
          <div class="ms-post-text">
            <p class="ms-post-date">04/03/2019</p>
            <h4 class="ms-post-title">Creating value beyond the deal</h4>
            <p class="ms-post-description">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. 
              Morbi feugiat, felis et sagittis pulvinar …
            </p>
          </div>

          <div class="ms-post-layer">
            <div class="ms-post-tags">
              <span class="badge">NEWS</span>
            </div>
            <p class="ms-post-date">04/03/2019</p>
            <h4 class="ms-post-title">Creating value beyond the deal</h4>
            <p class="ms-post-description">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. 
              Morbi feugiat, felis et sagittis pulvinar …
            </p>
          </div>
        </div>
        <div class="ms-post">
          <div class="ms-post-image">
            <img src="/img/home/last-new-1.jpg" alt="Last new post 1">
            <span class="badge">TOPICS</span>
          </div>
          <div class="ms-post-text">
            <p class="ms-post-date">04/03/2019</p>
            <h4 class="ms-post-title">Creating value beyond the deal</h4>
            <p class="ms-post-description">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. 
              Morbi feugiat, felis et sagittis pulvinar …
            </p>
          </div>

          <div class="ms-post-layer">
            <div class="ms-post-tags">
              <span class="badge">NEWS</span>
            </div>
            <p class="ms-post-date">04/03/2019</p>
            <h4 class="ms-post-title">Creating value beyond the deal</h4>
            <p class="ms-post-description">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. 
              Morbi feugiat, felis et sagittis pulvinar …
            </p>
          </div>
        </div>
    
      </div>
    </div>
    <div class="ms-button">
      <button class="ms-button-read-more">READ MORE NEWS</button>
    </div>
  </div>
</template>


<style lang="scss" scoped>
  .ms-latest-new {
    background-color: #ededed;

    .ms-background {
      display: flex;
      justify-content: space-between;

      img {
        width: 389.6px;
        height: 564.1px;
      }
    }

    .ms-title {
      position: relative;
      margin-top: -22vw;
      margin-left: 12vw;

      h1 {
        font-size: 40px;
        font-weight: bold;
        line-height: 1.48;
        color: #000;
        margin-left: 90px;
      }
    }

    .ms-title i{
      font-size: 10px;
      margin-left: 4px;
      color: #e82721;
    }

    .ms-icon {
      display: flex;
      justify-content: flex-end;
      padding-bottom: 50px;
      margin-right: 200px;
      font-size: 25px;
      margin-top: -4vw;
    }

    .ms-icon img{
      margin-right: 5vw;      
    }

    .ms-icon i:hover{
      color: #696969;
    }

    .badge {
      font-size: 11px;
      line-height: 1.18;
      letter-spacing: 0.88px;
      color: #fff;
      background-color: #000;

      padding: 6px 16px;
    }

    .ms-posts-wrapper {
      position: relative;
      bottom: -50px;
      z-index: 1;
      display: flex;
      justify-content: center;

    }

    .ms-posts {
      display: flex;
      justify-content: center;
      background-color: #fff;
      box-shadow: 0 -20px 20px 0 rgba(0, 0, 0, 0.04);
      padding: 30px;

      .ms-post {
        position: relative;
        width: 400px;
        margin-right: 20px;
        margin-bottom: 100px;
        
        &:last-child {
          margin-right: 0;
        }

        .ms-post-image {
          position: relative;
          height: 220px;
          overflow-y: hidden;

          img {
            width: 100%;
          }

          .badge {
            position: absolute;
            bottom: 15px;
            right: 30px;
          }
        }

        .ms-post-text {
          padding: 30px 15px 0 15px;
          height: 190px;
        }

        .ms-post-date {
          font-size: 11px;
          line-height: 1.18;
          letter-spacing: 0.88px;
          margin-top: 0;
          margin-bottom: 10px;
        }

        .ms-post-title {
          font-size: 23px;
          font-weight: bold;
          line-height: 1.17;
          margin-top: 0;
          margin-bottom: 10px;
        }

        .ms-post-description {
          font-size: 17px;
          line-height: 1.41;
          margin-top: 0;
        }

        .ms-post-layer {
          position: absolute;
          top: 0;
          left: 0;
          box-sizing: border-box;
          background-color: #e80023;
          width: 100%;
          height: 440px;
          display: none;
          padding: 25px 20px;

          .ms-post-tags {
            text-align: right;
            margin-bottom: 30px;
          }
        }

        &:hover {
          .ms-post-layer {
            display: block;
            
            .ms-post-date {
              color: #fff;
            }

            .ms-post-title {
              color: #fff;
            }

            .ms-post-description {
               color: #fff;
            }
          }
        }
      }
    }

    .ms-button {
      text-align: center;
      background-color: #fff;
      padding-top: 50px;
      margin-bottom: 100px;

      .ms-button-read-more {
        color: #fff;
        background-color: #000;
        font-size: 13px;
        font-weight: bold;
        line-height: 2.31;
        letter-spacing: 1.3px;
        padding: 25px 50px;
        border: none;
        cursor: pointer;
      }

      .ms-button-read-more:hover{
        background-color: #e82721;
      }
    }
  }
</style>