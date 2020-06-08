<template>
  <div>
      <div v-for="item in arr" v-bind:key="item">{{item}}</div>
      <div v-for="(item,index) in arr2" v-bind:key="index" >{{item.name}}</div>
      <div v-for="(item,key,index) in obj" v-bind:key="key" >
          <div>年:{{index}}-----{{item}}-----{{key}}</div>
      </div>
  </div>
</template>

<script>
export default {
    data(){
        return{
            arr:['苹果','香蕉','橘子'],
            arr2:[{name:'口红'},{name:"粉底"}],
            obj:{   
                age:10,
                msg:20,
                man:"四"     
            }
        }
    }
}
</script>

<style>

</style>