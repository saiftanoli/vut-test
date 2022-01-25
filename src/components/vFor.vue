<template>
<div>
    <h2 v-for="name in names" :key="name">{{name}}</h2>
    <h2 v-for="prof in profile" :key="prof">{{prof}}</h2>
    <h2 v-for="acting in actor" :key="acting">{{acting}}</h2>

    // conditional rendering elements
    <template v-for="ol in old" :key="ol">
       <h2 v-if="ol === 'asad'">{{ol}}</h2>
    </template>
</div>
</template>

<script>
export default {
    name: 'vFor',
    data() {
        return {
            names: ['saif', 'sunny', 'asad'],
            profile: [{
                    id: 1,
                    name: 'saif',
                    email: 'saif@gmail.com'
                },
                {
                    id: 2,
                    name: 'sunny',
                    email: 'sunny@gmail.com'
                }, {
                    id: 3,
                    name: 'asad',
                    email: 'asad@gmail.com'
                },
            ],
            actor: [{
                    name: 'srk',
                    movies: ['abx', 'dsf', 'asdda']
                },
                {
                    name: 'amir',
                    movies: ['abx', 'dsf', 'asdda']
                },
                {
                    name: 'salman',
                    movies: ['abx', 'dsf', 'asdda']
                },
            ],
            old: ['bruce', 'asad', 'telescope'],
        }
    }
}
</script>
