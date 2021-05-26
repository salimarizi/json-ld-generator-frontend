<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
    <SchemaGenerator msg="Sqwizi"/>
  </div>
</template>

<script>
import SchemaGenerator from './components/SchemaGenerator.vue'

export default {
  name: 'App',
  components: {
    SchemaGenerator
  }
}
</script>

<style>
  @import 'https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css';
  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    /* text-align: center; */
    color: #2c3e50;
    margin-top: 60px;
  }
</style>
