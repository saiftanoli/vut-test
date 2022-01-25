<template>
<div>
    <input v-model="first" type="number"><br>
    <input v-model="second" type="number"><br>

    <input v-model="result" type="number"><br>
    <button @click="plus()">+</button>
    <button @click="minus()">_</button>
    <button @click="multi()">*</button>
    <button @click="divide()">/</button><br><br>
</div>
</template>

<script>
export default {
    name: 'calculator',
    data() {
        return {
            first: '',
            second: '',
            result:'',
        }
    },
    methods: {
        plus() {
            this.result = 1  + 3 ; 
        }
    },

}
</script>
