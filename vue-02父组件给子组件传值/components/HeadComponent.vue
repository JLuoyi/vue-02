<template lang="">
    <div class="box">
        <span>首页</span>
        <input type="text"/>
        <div>搜索</div>{{posttitle}}
    </div>
</template>
<script>
export default {
    props:['posttitle'],
}
</script>
<style scoped>
    .box {
        display: flex;
        margin-top: 2%;
    }
    .box>input{
        width: 60%;
        margin-left: 5%;
        margin-right: 5%;
    }
</style>