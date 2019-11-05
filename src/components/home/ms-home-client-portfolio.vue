<template>
  <div class="ms-client-portfolio">
    <div class="ms-row">
      <div class="ms-text">
        <h1 class="ms-title">Client portfolio<i class="fa fa-square"></i></h1>
        
        <p class="ms-description">
          MY SPECTRUM clients have been installed in a 
          large number lorem ipsum over the past 20 years. 
          Here are some of our most important partners.
        </p>
      </div>
    </div>
    <div class="ms-logo">
      <img src="/partner-logo/com_03.png" alt="Coca Cola">
      <img src="/partner-logo/com_05.jpg" alt="NIKELODEON">
      <img src="/partner-logo/com_07.jpg" alt="Vodafone">
      <img src="/partner-logo/com_12.jpg" alt="Carlsberg">
      <img src="/partner-logo/com_14.jpg" alt="Mars">
      <img src="/partner-logo/com_16.jpg" alt="EONIKH">
      <img src="/partner-logo/com_21.jpg" alt="SAMSUNG">
      <img src="/partner-logo/com_23.jpg" alt="Cartier">
      <img src="/partner-logo/com_27.jpg" alt="Adidas">
      <img src="/partner-logo/com_28.jpg" alt="Anan">
      <img src="/partner-logo/com_22.jpg" alt="DIONIC">
      <img src="/partner-logo/com_11.jpg" alt="Notos">
      <img src="/partner-logo/com_09.jpg" alt="COSMOTE">
      <img src="/partner-logo/com_36.jpg" alt="AS Network">
      <img src="/partner-logo/com_13.jpg" alt="The Mall">
    </div>
    <div class="ms-button">
      <button class="ms-button-partner">VIEW ALL PARTNERS</button>
    </div>

    <!-- <div class="ms-particle-wrapper">
      <ms-particle
        width="400px"
        height="200px"
        link-color="#f2f2f2"
      ></ms-particle>
    </div> -->
  </div>
  
</template>

<script>
// import msParticle from '@/components/ms-particle.vue'

export default {
  // components: {
  //   msParticle
  // }
}
</script>

<style lang="scss" scoped>
.ms-client-portfolio {
  position: relative;
  background-color: #fff;

  .ms-row {
    width: 37vw;
    margin: 0 auto;
    display: flex;
    text-align: center;
  }
  .ms-title{
    height: 81.2px;
    font-family: Roboto;
    font-size: 40px;
    font-weight: bold;
    font-stretch: normal;
    font-style: normal;
    line-height: 1.48;
    letter-spacing: normal;
    text-align: center;
    color: #000000;
  }
  .ms-title i{
    font-size: 10px;
    margin-left: 4px;
    color: #e82721;
  }
  .ms-description{
    width: 716.1px;
    height: 75px;
    font-family: Roboto;
    font-size: 16px;
    font-weight: normal;
    font-stretch: normal;
    font-style: normal;
    line-height: 1.88;
    letter-spacing: normal;
    text-align: center;
    color: #000000;
  }
  .ms-logo{
    width: 89vw;
    margin-left: auto;
    margin-right: auto;
    margin-top: 112px;
  }
  .ms-logo img{
    width: 13vw;
    margin-right: 45px;
    margin-left: 45px;
    margin-top: 66px;
  }
  .ms-button-partner{
    width: 262.3px;
    height: 62px;
    background-color: #000000;
    color: #fff;
    font-family: Roboto;
    font-size: 13px;
    font-weight: bold;
    font-stretch: normal;
    font-style: normal;
    line-height: 2.31;
    letter-spacing: 1.3px;
    text-align: center;
    border: none;
  }
  .ms-button-partner:hover{
    background-color: #e82721;
  }
  .ms-button{
    width: 13.6%;
    margin-right: auto;
    margin-left: auto;
    margin-top: 197px;
  }

  .ms-particle-wrapper {
    position: absolute;
    bottom: 0;
    right: 0;
  }
}
</style>