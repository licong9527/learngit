<template>
  <div class="mz-tabbar">
    <ul class="mz-tabbar__ul">
      <li class="mz-tabbar__li">
        <a href>
          <i>图标</i>
          <span>电影</span>
        </a>
      </li>
      <li class="mz-tabbar__li">
        <a href>
          <i>图标</i>
          <span>影院</span>
        </a>
      </li>
      <li class="mz-tabbar__li">
        <a href>
          <i>图标</i>
          <span>特惠</span>
        </a>
      </li>
      <li class="mz-tabbar__li">
        <a href>
          <i>图标</i>
          <span>我的</span>
        </a>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "Tabbar"
};
</script>
<style lang="scss">
@import "../../assets/style/common/px2rem.scss";
.mz-tabbar {
  height: px2rem(50);
  background-color: #fff;
  &__ul {
    display: flex;
    height: 100%;
  }
  &__li {
    flex: 1;
    a {
      display: flex;
      flex-direction: column;
      align-items: center;
      text-decoration: none;
    }
  }
}
</style>
