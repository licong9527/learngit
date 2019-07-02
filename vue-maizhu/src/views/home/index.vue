<template>
  <div class="page-home">
    <router-view></router-view>
    <Tabbar
      :tabs="[
        { name: '电影', icon: 'icon-dianying', to: '/films' },
        { name: '影院', icon: 'icon-yingyuan', to: '/cinemas' },
        { name: '特惠', icon: 'icon-tehui', to: '/111' },
        { name: '我的', icon: 'icon-wode', to: '/center' }
      ]"
    />
  </div>
</template>
<script>
import Tabbar from "../../components/Tabber/index.vue";

export default {
  name: "home",

  components: {
    Tabbar
  }
};
</script>

<style lang="scss">
.page-home {
  height: 100%;
  display: flex;
  flex-direction: column;
  > div:first-child {
    flex: 1;
    overflow-y: auto;
  }
}
</style>
