<template>
  <a-layout-header class="home-header-wrapper">
    <logo />
    <div class="header-right">
      <HeadMenu />
    </div>
  </a-layout-header>
</template>

<script>
import HeadMenu from '@/views/rootHomePage/rootHeadMenu'
import Logo from '@/views/rootHomePage/rootHeaderLogo'

export default {
  name: 'RootHomeHeader',
  components: {
    HeadMenu,
    Logo
  },
  data () {
    return {}
  }
}
</script>

<style lang="less" scoped>
.home-header-wrapper {
  padding: 0 12px;
  background: #002140;
  color: white;
  display: flex;
  justify-content: space-between;
}
</style>
