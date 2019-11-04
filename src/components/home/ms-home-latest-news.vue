<template>
  <div class="ms-last-new">
    <div class="ms-background">
      <img src="@/assets/icons/page-last-new/intersection-15.png" alt="anc">
      <img src="@/assets/icons/page-last-new/intersection-16.png" alt="aanc">
    </div>
    <div class="ms-title">
      <h1>LATEST NEWS & INSIGHTS<i class="fa fa-square"></i></h1>
    </div>
    <div class="ms-icon">
      <a href="#"><i class="fa fa-arrow-left"></i></a>
      <a href="#"><i class="fa fa-arrow-right"></i></a>
    </div>
    <div class="ms-content">
      <div class="ms-post-1">
        <img src="/img/home/last-new-1.jpg" alt="Last new post 1">
        <p>04/03/2019</p>
        <h4>Creating value beyond the deal</h4>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. 
          Morbi feugiat, felis et sagittis pulvinar …
        </p>
      </div>
      <div class="ms-post-2">
        <div class="ms-post-2-btn">
            <button class="ms-post-2-btn-view">VIEWS</button>
          </div>
        <div class="ms-post-2-content">
          <p>04/03/2019</p>
          <h4>Creating value beyond the deal</h4>
          <p>
            Lorem ipsum dolor sit amet, consectetur 
            adipiscing elit. Morbi feugiat, felis et 
            sagittis pulvinar, lacus ligula dictum libero, 
            sit amet iaculis tellus neque sed justo. Ut vitae 
            magna ac enim facilisis porta vitae eget magna. Suspendisse molestie, 
          </p>
        </div>
      </div>
      <div class="ms-post-3">
        <img src="/img/home/last-new-2.png" alt="Last new post 1">
        <p>04/03/2019</p>
        <h4>Creating value beyond the deal</h4>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. 
          Morbi feugiat, felis et sagittis pulvinar …
        </p>
      </div>
    </div>
    <div class="ms-button">
      <button class="ms-button-read-more">READ MORE NEWS</button>
    </div>
  </div>
</template>


<style lang="scss" scoped>
  .ms-last-new{
    background-color: #ededed;
    .ms-background{
      display: flex;
      justify-content: space-between;
    }
    .ms-background img{
      width: 389.6px;
      height: 564.1px;
    }
    .ms-title{
      position: relative;
      margin-top: -22vw;
      margin-left: 12vw;
    }
    .ms-title i{
      font-size: 10px;
      margin-left: 4px;
      color: #e82721;
    }
    .ms-icon{
      display: flex;
      justify-content: flex-end;
      padding-bottom: 50px;
      margin-right: 200px;
      font-size: 25px;
      margin-top: -4vw;
    }
    .ms-icon i{
      margin-right: 5vw;
      color: #434343;
    }
    .ms-icon i:hover{
      color: #696969;
    }
    .ms-content{
      width: 68.5vw;
      background-color: #fff;
      display: flex;
      justify-content: center;
      padding-top: 30px;
      padding-left: 32px;
      padding-right: 32px;
      margin-left: auto;
      margin-right: auto;
      position: relative;
      box-shadow: 0 -20px 20px 0 rgba(0, 0, 0, 0.04);
    }
    .ms-post-1, .ms-post-3, .ms-post-2{
      width: 400px;
    }
    .ms-post-1, .ms-post-3, .ms-post-2{
      padding: 10px 10px 15px 10px;
    }
    .ms-post-1:hover, .ms-post-2:hover, .ms-post-3:hover{
      background-color: #e80023;
    }
    .ms-post-2{
      height: 462px;
      margin-left: 47px;
      margin-right: 47px;
      background-color: #e80023;
    }
    h4,p{
      padding-left: 10px;
    }
    h4{
      width: 369px;
      font-family: Roboto;
      font-size: 23px;
      font-weight: bold;
      line-height: 1.17;
      letter-spacing: normal;
      text-align: left;
      color: #000000;
      margin-bottom: 26px;
    }
    p{
      width: 368px;
      font-family: Roboto;
      font-size: 17px;
      font-weight: normal;
      line-height: 1.41;
      letter-spacing: normal;
      text-align: left;
      color: #000000;
      margin-bottom: -15px;
    }
    h1{
      width: 534.5px;
      height: 68.2px;
      font-family: Roboto;
      font-size: 40px;
      font-weight: bold;
      font-stretch: normal;
      font-style: normal;
      line-height: 1.48;
      letter-spacing: normal;
      text-align: left;
      color: #000000;
      margin-left: 90px;
    }
    img{
      width: 400px;
      height: 290px;
    }
    .ms-button{
      padding-top: 110px;
      padding-bottom: 116px;
      display: flex;
      justify-content: center;
      background-color: #fff;
      margin-top: -100px;
    }
    .ms-button .ms-button-read-more{
      color: #fff;
      width: 222.6px;
      height: 62px;
      background-color: #000000;
      font-family: Roboto;
      font-size: 13px;
      font-weight: bold;
      font-stretch: normal;
      font-style: normal;
      line-height: 2.31;
      letter-spacing: 1.3px;
      border: none;
      margin-top: 105px;
    }
    .ms-post-2-btn{
      display: flex;
      justify-content: flex-end;
    }
    .ms-post-2 .ms-post-2-btn-view{
      width: 64px;
      height: 27px;
      background-color: #000000;
      color: #fff;
      border: none;
      margin-top: 22px;
      margin-bottom: 22px;
      margin-right: 22px;
      position: relative;
    }
    .ms-post-2{
      background: #fff;
    }
   .ms-post-2-content h4,p{
     color: #000;
   }
    
  }
</style>