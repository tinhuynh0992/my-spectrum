<template>
  <div :class="{ 'ms-lang-switcher': true, 'active': isOpen }" @click="toggleLangSwitcher">
    <div class="ms-lang-current">{{ currentLang }}</div>
    <div class="ms-lang-icon"><i class="fa fa-caret-down"></i></div>
    <div class="ms-lang-dropdown">
      <ul class="ms-langs">
        <li class="ms-lang" @click="changeLang('En')">En</li>
        <li class="ms-lang" @click="changeLang('Fr')">Fr</li>
      </ul>
    </div>    
  </div>  
</template>

<script>
export default {
  data() {
    return {
      isOpen: false,
      currentLang: 'En'
    }
  },

  methods: {
    toggleLangSwitcher() {
      this.isOpen = !this.isOpen
    },

    changeLang(lang) {
      this.currentLang = lang
    }
  }
}
</script>

<style lang="scss" scoped>
.ms-lang-switcher {
  width: 80px;
  height: 80px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  position: relative;
  cursor: pointer;

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

  .ms-lang-dropdown {
    position: absolute;
    top: 60px;
    opacity: 0;

    .ms-langs {
      margin: 0;
      padding: 0;

      li {
        list-style-type: none;
        margin-bottom: 10px;
        font-size: 14px;
        font-weight: bold;
        line-height: 1.14;
        letter-spacing: 2.8px;
        color: #fff;
        cursor: pointer;
      }
    }
  }

  &.active {
    .ms-lang-dropdown {
      opacity: 1;
    }
  }
}
</style>