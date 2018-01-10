<template>
  <div id="app">
    <GridRow />
    <GridRow :isCommunicationRow="true" />
    <GridRow />
    <TestControlls />
  </div>
</template>

<script lang="ts">
import Vue from 'vue';
import Component from 'vue-class-component';

import GridRow from './components/gridRow.vue';
import TestControlls from './components/testControlls.vue';

@Component({
  components:{
    GridRow,
    TestControlls
  }
})
export default class App extends Vue {
}
</script>

<style>
html, body{
  background-color: black;
  width: 100%;
  height: 100%;
  padding:0;
  margin:0;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  height: 90%;
  padding:0;
  margin:0;
}
</style>
