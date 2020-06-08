<template>
  <div>
      <h1 v-if='flag'>我是大学生</h1>
      <h1 v-if='flag2'>我是小流氓</h1>
      <p v-if="month>=2&&month<=4">春天</p>
      <p v-else-if="month>4&&month<=7">夏天</p>
      <p v-else-if="month>7&&month<=10">秋天</p>
      <p v-else>冬天</p>
      <p>{{month}}</p>
  </div>
</template>

<script>
export default {
    data(){
        return{
            flag:true,
            flag2:false,
            month1:1,
            month:6
        }
    }
}
</script>

<style>

</style>