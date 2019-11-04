<template>
  <div class="ms-lang-switcher">
    <div class="ms-lang-current">En</div>
    <div class="ms-lang-icon"><i class="fa fa-caret-down"></i></div>
  </div>  
</template>

<style lang="scss" scoped>
.ms-lang-switcher {
  width: 80px;
  height: 80px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;

  .ms-lang-current {
    font-size: 14px;
    font-weight: bold;
    line-height: 1.14;
    letter-spacing: 2.8px;
    color: #fff;
  }

  .ms-lang-icon {
    font-size: 16px;
    line-height: 1.06;
    letter-spacing: 1.6px;
    color: #fff;
  }
}
</style>