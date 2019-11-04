<template>
  <div
    :style="{
      width: width,
      height: height
    }"
    ref="particle"
  >
  </div>
</template>

<script>
export default {
  props: {
    width: {
      type: String,
      default: '100px'
    },
    height: {
      type: String,
      default: '100px'
    },
    numberParticles: {
      type: Number,
      default: 10
    },
    particleColor: {
      type: String,
      default: '#e82721'
    },
    linkColor: {
      type: String,
      default: '#efecec'
    }
  },

  mounted() {
    if (window.jQuery) {
      window.jQuery(this.$refs.particle).jParticle({
        background: "transparent",
        color: this.linkColor,
        particlesNumber: this.numberParticles,

        particle: {
          color: this.particleColor,
          minSize: 10,
          maxSize: 10
        }
      })
    }
  }
}
</script>