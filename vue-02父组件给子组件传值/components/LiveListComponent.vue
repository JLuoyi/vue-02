<template lang="">
    <div class="liveBox">
        <live v-for="num in 6"></live>
    </div>
</template>
<script>
import live from '@/view/LiveItem.vue';
export default {
    components:{
        live
    }
}
</script>

<style scoped>
    .liveBox {
        width: 100%;
        min-height: 400px;
        background-color: deepskyblue;
        margin-top: 2%;
        padding-left: 5%;
        padding-right: 5%;
        display: flex;
        flex-wrap: wrap;
        justify-content: space-between;
    }
</style>