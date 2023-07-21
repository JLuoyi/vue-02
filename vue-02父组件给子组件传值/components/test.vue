<template lang="">
    <div>
        <button @click="qh()">切换</button>
    </div>
</template>
<script>
import cha from './chacao.vue';
export default {
    components:{
        cha
    },
    data() {
        return {
            change:'A'
        }
    },
    methods:{
        qh(){
            this.change = this.change == 'A' ? 'B':'A';
        }
    }
}
</script>
<style lang="">
    
</style>