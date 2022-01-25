<template>
<div>
    <h1 ref="user">test</h1>
</div>
</template>

<script>

export default {
    name: 'unMount',
     beforeUnmount() {
        console.log('before unmount' , this.$refs['user']);
    },
    unmounted(){
        console.log('before unmount' , this.$refs['user']);
    }
}
</script>

<style lang="scss" scoped>

</style>
