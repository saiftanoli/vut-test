<template>
<div>
    <c-child :getUserName="getUserName" name="name" />
    {{name}}
</div>
</template>

<script>
import cChild from './cChild.vue'
export default {
    components: {
        cChild
    },
    methods: {
            getUserName(name){
                alert(name)
            }
        },

}
</script>

<style lang="scss" scoped>

</style>
