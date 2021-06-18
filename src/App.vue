<template>
  <div id="app">
    <div class="box" v-for="(box, i) in boxes" :key="i">{{i + 1}}</div>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      boxes: 9
    }
  }
}
</script> 

<style>
.box {
  width: 50px;
  height: 50px;
  border: 1px solid black;
  margin: 5px;
  display: flex;
  justify-content: center;
  align-items: center;
  }
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  display: flex;
  justify-content: center;
  align-items: top;
  flex-wrap: wrap;
  flex-direction: reverse;
}
</style>
