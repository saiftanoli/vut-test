<template>
<div>
    <h1>parent</h1>
    <child name="saif" :user="user" :getData="getData" />
</div>
</template>

<script>
import child from './child.vue'
export default {
    components: {
        child
    },
    name: 'parent',
    data() {
        return {
            user: [{
                name: 'saif',
                email: 'saif@gmail.com'
            }],
            name:''
        }
    },
    methods: {
        getData(){
            console.log("sunny")
        }
    },
}
</script>
