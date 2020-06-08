<template>
  <div id="app">
    <!-- <Moden /> -->
    <!-- <Tiaojian /> -->
    <!-- <List /> -->
    <Event />
  </div>
</template>

<script> 
import Moden from "./components/moden"
import Tiaojian from "./components/tiaojian"
import List from "./components/list"
import Event from "./components/event"
export default {
  name: 'App',
  components: {
    Moden,
    Tiaojian,
    List,
    Event
  }
}
</script>

<style lang="less">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
