<template>
  
  <div id="app">

    <nestedone message="This is message one..." :number="1"></nestedone>
    <nestedone message="This is message two..."></nestedone>
    <nestedone></nestedone>

  </div>

</template>

<script>

  import  nestedone from './components/NestedOne';

  export default {
    name: 'app',
    components: {
      nestedone
    }
  }

</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
