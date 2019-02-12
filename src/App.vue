<template>
      <div id="app">
        <h1>Data visualisation with Vue.js</h1> 
        <visualisation></visualisation>
      </div>
    </template>
    <script>
    /* eslint-disable */
    import Visualisation from './components/Visualisation.vue';

    export default {
      name: 'app',
      components: {
        Visualisation
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