<template>
  <h1> Pass data to child component</h1>
  <Child name="Vijay Mane" :user="user" :getData="getData" />
</template>

<script>
import Child from './Child.vue'
export default {
    name :"Parent-Data",
    components:{
        Child
    },
    data(){
        return{
            user:{
                name: "vijay",
                email:"vijay@gmail.com"
            }
        }
    },
    methods:{
        getData(){
            console.log("parent function called")
            alert('hello');
        }
    }
}
</script>

<style>

</style>