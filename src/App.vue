<template lang="">
    <div>
        父组件,来自子组件的数据:{{message}}
        <son :cjb="cjb" v-on:suibian="receiveMessage"></son>
    </div>
</template>
<script>
import son from './components/sonCompnent.vue';
export default {
    provide:{
        jz:"<<真金>>"
    },
    data() {
        return {
            message:"",
            cjb:"金子"
        }
    },
    components:{
        son
    },
    methods:{
        receiveMessage(data){
            console.log(data);
            this.message=data
        }
    }
}
</script>
<style lang="">
    
</style>
