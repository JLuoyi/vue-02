<template lang="">
  <div>
    <Head posttitle="hello"></Head>
    <Banner></Banner>
    <Classify :menuList="menuList"></Classify>
    <LiveLIst></LiveLIst>
    <Bar></Bar>
  </div>
</template>
<script>
import Head from './components/HeadComponent.vue';
import Banner from './components/BannerComponent.vue';
import Classify from './components/ClassifyComponent.vue';
import LiveLIst from './components/LiveListComponent.vue';
import Bar from './components/BarComponent.vue';
export default {
  // 注册组件
  components: {
    Head,
    Banner,
    Classify,
    LiveLIst,
    Bar
  },
  data() {
    return {
      menuList: []
    }
  },
  mounted() {
    this.initClassify();
  },
  methods: {
    initClassify() {
      this.menuList = [
        { menuIcon: "", title: "全部" },
        { menuIcon: "", title: "靓仔啊" },
        { menuIcon: "", title: "靓女啊" }
      ]
    }
  },
}
</script>
<style scoped>
* {
  margin: 0;
  padding: 0;
  list-style: none;
  box-sizing: border-box;
}
</style>
