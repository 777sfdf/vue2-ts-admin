<template>
    <!-- <h2>右边内容区域页面</h2> -->
    <div>
    <!-- 顶部区域 -->
        <Header></Header>
        <!-- 内容区域 -->

        <router-view></router-view>
    </div>
</template>

<script>
import Header from './Header.vue'

export default{
    components:{
        Header
    }
}
</script>
<style>

</style>