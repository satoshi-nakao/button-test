<template>
  <div>
    <h1>{{ message }}</h1>
    <button @click="countup">+</button>
    <button @click="countdown">-</button>
    <P>{{ number1 }}</P>
    <p>{{ number2 }}</P>
  </div>
</template>

<script>

export default {
  data() {
    return{
      message : "ボタンのテスト",
      number1 : 0,
      number2 : 12000
    }
  },
  methods: {
    countup() {
      this.number1 += 1
    },
    countdown() {
      this.number2 -= 1
    }
  }
}
</script>

<style>
/* #app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
} */
</style>
