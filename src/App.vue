<template>
  <div id="app">
    調べたい年：<input type="text" v-model="year"><br>

  </div>
</template>

<script>
export default {
  data() {
    return {
      year: 0,
      
    };
  },
  methods: {
    leapYear(year) {
      if( (year % 4 === 0 && year % 100 !== 0) || year % 400 === 0) {
        console.log("うるう年")
      } else{
        console.log("うるう年ではありません")
}
    }
  }
};
    

</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
