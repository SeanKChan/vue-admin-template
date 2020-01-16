<template>
  <section class="app-main" :style="style">
    <transition name="fade-transform" mode="out-in">
      <router-view :key="key" />
    </transition>
  </section>
</template>

<script>
import WaterMark from '@/utils/waterMark'

export default {
  name: 'AppMain',
  data() {
    return {
      style: null
    }
  },
  computed: {
    key() {
      return this.$route.path
    },
    userName() {
      return this.$store.state.user.name
    },
    waterMarkStyle() {
      return this.$store.state.app.waterMarkStyle
    }
  },
  mounted() {
    if (_.isEmpty(this.waterMarkStyle)) {
      const imgBase64 = WaterMark(this.userName)
      const style = {
        background: `url(${imgBase64})`
      }
      this.$store.dispatch('app/setWaterMarkStyle', style)
    }
    this.style = this.waterMarkStyle
  }
}
</script>

<style scoped>
.app-main {
  /*50 = navbar  */
  min-height: calc(100vh - 50px - 43px);
  width: 100%;
  position: relative;
  overflow: hidden;
}
.fixed-header + .app-main {
  padding-top: 50px;
}
</style>

<style lang="scss">
// fix css style bug in open el-dialog
.el-popup-parent--hidden {
  .fixed-header {
    padding-right: 15px;
  }
}
</style>
