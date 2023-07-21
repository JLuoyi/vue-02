<template lang="">
    <div>
        大壮:{{cjb}}<br>
        <!-- <button @click="sendMessage">传递数据</button> -->
        <input type="text" v-model="message" @keydown="sendMessage">
        <Grandson :cjb="cjb"></Grandson>
</div>
</template>
<script>
import Grandson from './GrandsonComponent.vue';
export default {
    props:["cjb"],
    data() {
        return {
            message:""
        }
    },
    methods:{
        sendMessage(){
            this.$emit('suibian',this.message);
        }
    },
    components:{
        Grandson
    }
    
}
</script>
<style lang="">
    
</style>