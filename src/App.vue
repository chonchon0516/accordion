<template>
  <div id="app">
    調べたい年：<input type="text" v-model="year"><br>
<button v-on:click="leapYear">調べたい年</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      year: "";
    };
  },
  computed: {
    double() {
      return this.number * 2;
    },
    numberClass() {
      if (this.number > 50) {
        return "red";
      }

      return "blue";
    }
  },
  methods: {
    leapYear(year) {
      if((this.year % 4 == 0 && this.year % 100 !== 0) || this.year % 400 == 0)
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
