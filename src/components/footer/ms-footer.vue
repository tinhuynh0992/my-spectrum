<template>
  <footer>
    <div class="ms-footer">
      <div class="ms-icon">
        <img src="@/assets/icons/footer/placeholder-image.jpg" alt="icon-footer" class="Intersection-14">
      </div>
      <div class="ms-container-left">
        <h4>Get in Touch</h4>
        <p>Kifissias Avenue 189 Marousi, 15124, Greece</p>
        <p>T.  +30 210 7237105 E. info@my-spectrum.com</p>
        <i class="fa fa-facebook"></i>
        <i class="fa fa-twitter"></i>
        <i class="fa fa-linkedin"></i>
        <i class="fa fa-vimeo"></i>
      </div>
      <div class="ms-container-right">
        <h4>Subscribe to our Newsletter</h4>
        <p> By subscribing here, you will receive our newsletters. You can unsubscribe at any time by following the link at the bottom of each newsletter. </p>
        <div class="ms-container-right-box">            
          <input type="text" id="txt-container-right-email" placeholder="Type your email/here" onfocus="this.placeholder = ''" onblur="this.placeholder = 'Type your email/here'" >
          <button class="ms-container-right-icon"><i class="fas fa-long-arrow-alt-right"></i></button>
        </div>
        <div class="ms-container-right-link">
          <a href="#">PRIVACY POLICY</a> 
          <a href="#">TERMS OF USE</a> 
          <a href="#">COOKIES POLICY</a> 
        </div>
      </div>
      <div class="ms-container-bottom-right">
        <a href="#" >TO TOP</a>
        <hr class="new1">
      </div>

    </div>
  </footer>  
</template>

<style lang="scss" scoped>
  h4{
      width: 250px;
      height: 24px;
      font-family: Roboto;
      font-size: 20px;
      font-weight: bold;
      font-stretch: normal;
      font-style: normal;
      line-height: 1.5;
      letter-spacing: normal;
      text-align: left;
      color: #fff;
      padding-top: 92px;
      padding-bottom: -46px;
    }
  p{
    width: 180px;
    height: 43px;
    font-family: Roboto;
    font-size: 15px;
    font-weight: normal;
    font-stretch: normal;
    font-style: normal;
    line-height: 1.67;
    letter-spacing: normal;
    text-align: left;
    color: #fff;
    margin-bottom: 46px;
  }
  i{
    width: 8px;
    color: #969392;
    margin-right: 39px;
    margin-top: 39px;
    font-size: 25px;
  }
  .ms-footer{
    display: flex;
    justify-content: flex-start;
    background-color: #000;
  }
  .Intersection-14 {
    width: 366.3px;
    height: 421.6px;
    background-color: #2b2b2b;
  }
  .ms-container-right{
    margin-right: auto;
  }
  .ms-container-right p{ 
    width: 491.3px;
    color: #969392;
  }
  .ms-container-right-icon{
    position: absolute;
    align-items: center;
    height: 70px;
    background-color: transparent;
    border: none;
  }
  .ms-container-right-box input#txt-container-right-email:hover, .ms-container-right-box input#txt-container-right-email:focus, .ms-container-right-box input#txt-container-right-email:active{
    outline:none;
  }
  .ms-container-right-box input#txt-container-right-email{
    width: 491.3px;
    height: 66px;
    background: #000;
    border: none;
    font-size: 10pt;
    float: left;
    color: #fff;
    padding-left: 15px;
    -webkit-border-radius: 5px;
    -moz-border-radius: 5px;
    border-radius: 5px;
    border: solid 1px #707070;
    
  }
  .ms-container-right-box{
    width: 491.3px;
    height: 66px;
    vertical-align: middle;
    white-space: nowrap;
    display: flex;
    justify-content: flex-end;
  }
  .ms-container-right-box input#txt-container-right-email::-webkit-input-placeholder {
   color: #fff;
  }
  
  .ms-container-right-box input#txt-container-right-email:-moz-placeholder { /* Firefox 18- */
    color: #fff;  
  }
  
  .ms-container-right-box input#txt-container-right-email::-moz-placeholder {  /* Firefox 19+ */
    color: #fff;  
  }
  
  .ms-container-right-box input#txt-container-right-email:-ms-input-placeholder {  
    color: #fff;  
  }
  .ms-container-right-icon i{
    margin-top: inherit;
    margin-right: 20px;
  }
  .ms-container-right-icon i:hover{
    color: #fff;
  }
  .ms-container-left i:hover{
    color: #fff;
  }
  .ms-container-right-link{
    margin-top: 66px;
  }
  .ms-container-right-link a{
    margin-right: 10px;
    font-family: Roboto;
    font-size: 13px;
    font-weight: normal;
    font-stretch: normal;
    font-style: normal;
    line-height: 1.92;
    letter-spacing: 0.65px;
    color: #969392;
    text-decoration: none;
  }
  .ms-container-right-link a:hover{
    color: #fff;
  }
  .ms-container-bottom-right{
    transform: rotate(-90deg);
    -moz-transform: rotate(-90deg);
    -webkit-transform: rotate(-90deg);
    -o-transform: rotate(-90deg);
    display: flex;
    align-items: center;
  }
  .ms-container-bottom-right a{
    margin-left: 65px;
    height: 68px;
    font-family: Roboto;
    font-size: 10px;
    font-weight: bold;
    font-stretch: normal;
    font-style: normal;
    line-height: 1.1;
    letter-spacing: 3px;
    text-align: left;
    color: #fff;
    text-decoration: none;
  }
</style>