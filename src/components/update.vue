<template>
    <div>
        <h2 ref="count">{{counter}}</h2>
        <button  @click="counter += 2">add</button>
    </div>
</template>

<script>
    export default {
        name:'update',
        data() {
            return {
                counter: 0,
            } 
        },
         beforeUpdate() {
             console.log('beforeUpdate' ,this.$refs['count'].textContent) ; 
            },
            updated(){
                console.log('Updated' ,this.$refs['count'].textContent) ; 
            }
    }
</script>

<style lang="scss" scoped>

</style>