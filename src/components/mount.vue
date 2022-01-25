<template>
    <div>
        {{name}}
    </div>
</template>

<script>
    export default {
        name:'mount',
        data() {
            return {
                name: 'sunny'
            }
        },
        beforeMount() {
            console.log('beforeMount', this.$el)
        },
        mounted(){
            this.name='saif';
            console.log('mounted', this.$el)
        }
    }
</script>

<style lang="scss" scoped>

</style>