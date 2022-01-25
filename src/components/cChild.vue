<template>
    <div>
<button @click="getUserName(userName)"> user</button>
    </div>
</template>

<script>
    export default {
        name:'cChild',
        data() {
            return {
                userName: 'saif',
                name:'sunny'
            }
        },
        props:{
            getUserName:Function,
        }
    }
</script>
