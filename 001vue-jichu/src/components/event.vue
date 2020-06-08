<template>
  <div>
      <button v-on:click="clickme('woai','北京',2,$event)">传参</button>
      <a href="https://www.baidu.com/" v-on:click.prevent="clickme1">百度</a>
      <div>
          {{num}}
          {{num1}}
      </div>
       <button v-on:click="xiugai">修改</button>
  </div>
</template>

<script>
export default {
    data(){
        return{
            num:0,
            num1:0
        }
    },
    methods:{
        clickme(...item){
            console.log(item)
        },
        clickme1(){
            console.log("找百度去啊")
            console.log( this.num1)

            
        },
        xiugai(){
            this.num+=5
            this.num1="我的天哪"
        }
    }
}
</script>

<style>

</style>