<template>
    <div>
        {{count}}
        <button @click="count += 1">add count</button>
        <button @click="count -= 1">sub count</button>
    </div>
</template>

<script>
    export default {
        name:'watcher',
        data() {
            return {
                count: 0,
            }
        },
        watch :{
            count(value , old){
                if(value >= 10 && value>old){
                    alert('its is a limit')
                }
            }
        }
    }
</script>

<style lang="scss" scoped>

</style>