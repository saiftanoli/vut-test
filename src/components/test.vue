<template>
<div>
    <button @click="show =!show">toogle</button>
    <un-mount v-if="show" />
</div>
</template>

<script>
import unMount from './unMount.vue'
export default {
    name: "test",
    data() {
        return {
            show: true
        }
    },
    components:{
        unMount
    },
   
    

}
</script>

<style lang="scss" scoped>

</style>
