<template>
  <div>
    <tab-bar>
      <tab-bar-item v-slot:item class="tab-bar-item">
        <router-link to="/home" tag="div">
          <i class="iconfont icon-home"></i>
          <span>首页</span>
        </router-link>
      </tab-bar-item>
      <tab-bar-item v-slot:item class="tab-bar-item">
        <router-link to="/category" tag="div">
          <i class="iconfont icon-goods"></i>
          <span>分类</span>
        </router-link>
      </tab-bar-item>
      <tab-bar-item v-slot:item class="tab-bar-item">
        <router-link to="/cart" tag="div">
          <i class="iconfont icon-cart"></i>
          <span>购物车</span>
        </router-link>
      </tab-bar-item>
      <tab-bar-item v-slot:item class="tab-bar-item">
        <router-link to="/profile" tag="div">
          <i class="iconfont icon-people"></i>
          <span>我的</span>
        </router-link>
      </tab-bar-item>
    </tab-bar>
  </div>
</template>

<script>
import TabBar from "./TabBar";
import TabBarItem from "./TabBarItem";
export default {
  data() {
    return {};
  },
  components: {
    TabBar,
    TabBarItem
  },
  created() {},
  methods: {}
};
</script>

<style lang="scss" scoped>
@import url("//at.alicdn.com/t/font_1842003_32zvyosyp3u.css");
.iconfont {
  font-size: 20px;
}

.tab-bar-item {
  flex: 1;
  text-align: center;
  div {
    height: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    span {
      font-size: 14px;
    }
  }
}
.active-bar {
  color: red;
}
</style>
