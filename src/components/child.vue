<template>
<div>
    <h1>child component</h1>
    {{name}}
    {{user}}
    <button @click="getData()">get</button>
    
</div>
</template>

<script>
export default {
    name: 'child',
    props: {
        name: String,
        user:Array,
        getData: Function,
    }
    
}
</script>

<style lang="scss" scoped>

</style>
