<template>
    <div>
        {{name}}
    </div>
</template>

<script>
    export default {
        name:'beforeCreate',
        data() {
            console.log('just for testing');
            return {
                name: 'sunny'
            }
        },
        beforeCreate() {
            alert('before creation')
        },
        created(){
            this.name='saif';
            alert('after the creation')
        }
    }
</script>




<style lang="scss" scoped>

</style>