<template>
  <footer class="ms-footer">
    <div class="ms-particle-wrapper">
      <ms-particle
        width="300px"
        height="400px"
      ></ms-particle>
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
      <p> 
        By subscribing here, you will receive our newsletters. 
        You can unsubscribe at any time by following the link at 
        the bottom of each newsletter. 
      </p>
      <div class="ms-container-right-box">            
        <input type="text" id="txt-container-right-email" placeholder="Type your email/here" onfocus="this.placeholder = ''" onblur="this.placeholder = 'Type your email/here'" >
        <button class="ms-container-right-icon"><i class="fa fa-long-arrow-alt-right"></i></button>
      </div>
      <div class="ms-container-right-link">
        <a href="#">PRIVACY POLICY</a> 
        <a href="#">TERMS OF USE</a> 
        <a href="#">COOKIES POLICY</a> 
      </div>
    </div>
    <div class="ms-footer-bottom-right">
      <span @click="handleScrollUp">TO TOP</span>
      <hr class="ms-footer-bottom-right-line">
    </div>

  </footer>
</template>

<script>
import msParticle from '@/components/ms-particle.vue'

export default {
  methods: {
    handleScrollUp() {
      console.log("Click on scroll up");
    }
  },
  components: {
    msParticle
  }
}
</script>

<style lang="scss" scoped>
.ms-footer{
  width: 100%;
  position: relative;
  overflow-x: hidden;
  display: flex;
  align-items: flex-end;
  background-color: #000;

  .ms-particle-wrapper {
    height: 350px;
    overflow: hidden;
  }

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
    color: #969392;
    margin-bottom: 46px;
  }
  i{
    width: 8px;
    color: #969392;
    margin-right: 39px;
    margin-top: 39px;
    font-size: 25px;
  }
  .Intersection-14 {
    width: 366.3px;
    height: 421.6px;
    background-color: #2b2b2b;
  }
  .ms-container-right{
    margin-left: 22vw;
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
  }
  .ms-container-right-icon i:hover, .ms-container-right-icon i:active, .ms-container-right-icon i:focus{
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
  .ms-footer-bottom-right {
    position: absolute;
    top: 0;
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

    .ms-footer-bottom-right-line {
      width: 125px;
      margin-left: 30px;
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