<template>
    <!-- <h2>右边内容区域页面</h2> -->
    <div>
    <!-- 顶部区域 -->
    <div class="header">
     <div class="open">
     <span v-if="!isCollapse" class="iconfont icon-zhedie1" @click="changeMenu"></span>
     <span v-else="isCollapse" class="iconfont icon-zhedie2" @click="changeMenu"></span>
    
    </div>
     </div>


        <!-- 内容区域 -->
        <router-view></router-view>
    </div>
</template>

<script>


export default{
    props: ['isCollapse'],
   
    methods:{
        changeMenu(){
            this.$emit('changeShow')
        }
    }
}
</script>
<style>
.header{
    height: 50px;
    background: #1e78bf;
    color: #fff;
    line-height: 50px;
    .open{
        .iconfont{
            font-size: 22px;   
        }
       
        
    }
}
</style>