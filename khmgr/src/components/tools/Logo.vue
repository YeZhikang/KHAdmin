<template>
  <div class="logo">
    <router-link :to="{ name: 'rootHomePage' }">
      <LogoSvg alt="logo" />
      <h1 v-if="showTitle">{{ $t('khmgr.name') }}</h1>
    </router-link>
  </div>
</template>

<script>
import LogoSvg from '@/assets/icon.svg?inline'

export default {
  name: 'Logo',
  components: {
    LogoSvg
  },
  props: {
    title: {
      type: String,
      default: '健康护航',
      required: false
    },
    showTitle: {
      type: Boolean,
      default: true,
      required: false
    }
  }
}
</script>

<style lang="less" scoped>
.logo {
  display: flex;
  justify-content: center;
}
</style>
