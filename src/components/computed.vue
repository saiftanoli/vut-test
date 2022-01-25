<template>
<div>
    <h2>{{fname}} {{lname}}</h2>
    <h2>{{fullname}}</h2>
    <h2>{{total()}}</h2>
</div>
</template>

<script>
export default {
    name: 'computed',
    data() {
        return {
            fname: 'saif',
            lname: 'ullah',
            items: [{
                    id: 1,
                    title: 'tv',
                    price: '100',
                },
                {
                    id: 2,
                    title: 'mobile',
                    price: '200',
                },
                {
                    id: 3,
                    title: 'laptop',
                    price: '300',
                },
            ],
        }
    },
    methods: {},
    computed: {
        fullname() {
            return `${this.fname} ${this.lname}`
        },
        total(){
            return this.items.reduce((total , curr) => (total = total + curr.price),0)
        }
    }
}
</script>


