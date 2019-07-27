<template>
  <div id="app">
    <Calculator/>
  </div>
</template>

<script>
import Calculator from './components/Calculator';

export default {
  name: 'app',
  components: {
    Calculator
  }
}
</script>

<style scaped>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.calculator {
  margin: 0 auto;
  width: 400px;
  font-size: 30px;
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  grid-auto-rows: minmax(50px, auto);
}
.calculator div {
  line-height: 50px;
}
.display {
  grid-column: 1 / 5;
  background-color: #333;
  color: white;
  height: 70px;
  line-height: 70px !important;
}
.zero {
  grid-column: 1 / 3;
}
.btn {
  background-color: #F2F2F2;
  border: 1px solid #999;
}
.operator {
  background-color: orange;
  color: white;
}
</style>
