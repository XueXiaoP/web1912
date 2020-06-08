<template>
  <div>
     hello word
    <h3>{{title}}</h3>
    <p>{{dome(50,50)}}</p>
    <p>{{1>2?"成功":"失败"}}</p>
    <p>{{price}}</p>
    <p v-html='price'></p>
    <p v-html='"<h1>松花江上</h1>"'></p>
  </div>
</template>

<script>
export default {
    name:'moden',
     data(){
        return {
            title:"我家在东北",
            price:"<h3>30000</h3>"
        }
    },
  methods:{
    dome(a,b){
        return a+b
    }
  },
   components: {
   
  }
}
</script>

<style>

</style>