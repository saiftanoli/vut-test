<template>
    <h1 v-if="number > 0">is a positive number.</h1>
    <h1 v-else-if="number < 0">is a negative number.</h1>
    <h1 v-else-if="number === 0"> number is zero.</h1>
    <h1 v-else>not a number</h1>
    
    <label > Enter your cnic number</label>
    <input @keyup.enter="cal()" v-model="num" type="number">

    <div  v-if="num === 12345 " >
          {{info}}
    </div>
    
</template>

<script>
export default {
  name: 'HelloWorld',
  data() {
    return {
      number: '0',
      num:true,
      info: []
    }
  },
  methods: {
    cal() {
      this.info=[{
        name:'saif',
        email:'saif@gmail.com' ,
        city:'mansehra',
        phone:'0034537452',
        }];
    }
  },
 
}
</script>