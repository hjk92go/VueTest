<script>
export default {
  data() {
    return {
      numberClass:"number",
      count: 5
    }
  },
  methods : {
      increment() {
        this.count++
      }
    }
}
</script>

<template>
  <H1 v-bind:class="numberClass" >    {{count}}  </H1>
  <h1>vue로 확인하는 웹페이지 입니다. 아래 버튼을 누르면 값이 1씩 증가합니다.</h1>
<button v-on:click="increment" v-bind:class="numberClass+1">1+</button>
</template>

<style>
  .number{
    font-size:70px;
    color: red;
    font-weight: 400;
  }

  .number1{
    border: solid 5px black;
    border-radius: 20%;
    font-size: x-large;
    color: black;
    width: 70px;
    height: 50px;
    margin-top: 15px;

  }
</style>