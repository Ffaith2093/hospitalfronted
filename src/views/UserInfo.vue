<!--
 * @Description: to check and modify user's infomation
 * @Author: y
-->
<template>
    <div>
        <Hearder />
        <p>test</p>
        <Footer />
    </div>
</template>
<script>
    import Hearder from "../components/header.vue";
    import CardList from "../components/cardList.vue";
    import Footer from "../components/footer.vue";
    export default {
    name: "UserInfo",
    components: {
      Hearder,
      CardList,
      Footer,
    },
    data() {
    return {}
    }
}
</script>
<style lang="less" scoped>
</style>