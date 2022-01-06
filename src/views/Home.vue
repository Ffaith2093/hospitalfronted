<!--
 * @Description: file information
 * @Author: Dzl
 * @Date: 2021-08-22 10:51:03
 * @LastEditors: Dzl
 * @LastEditTime: 2021-11-11 08:40:02
-->
<template>
  <div id="web">
    <Hearder />
    <Banner />
    <IntroContent />
    <CardList />
    <Content />
    <Footer />
  </div>
</template>

<script>
import Hearder from "../components/header.vue";
import Banner from "../components/banner.vue";
import IntroContent from "../components/introContent.vue";
import Content from "../components/contents.vue";
import CardList from "../components/cardList.vue";
import Footer from "../components/footer.vue";
export default {
  name: "Home",
  components: {
    Hearder,
    Footer,
    Banner,
    Content,
    IntroContent,
    CardList,
  },
  data() {
    return {
      list: [{}, {}, {}, {}],
    };
  },
  created() {},
  methods: {
    seeMore() {
      this.$message.warning("此功能暂未开放");
    },
  },
  mounted() {},
};
</script>
<style lang="less">
</style>
