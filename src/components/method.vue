<template>
    <div>
        <h2>{{add(2,3,4)}}</h2>
        <h2>{{ multiply(6) }}</h2>
    </div>
</template>

<script>
    export default {
        name:'method',
        data() {
            return {
                number: 5,
            }
        },
        methods: {
            add(a,b,c) {
                return a+b+c;
            },
        multiply(num){
            return  num * this.number ;
        },
    }
    }
</script>

<style lang="scss" scoped>

</style>