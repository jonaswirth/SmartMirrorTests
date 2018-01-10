<template>
  <div id="app">
    <GridRow />
    <GridRow :isCommunicationRow="true" />
    <GridRow />
    <div class="test-controlls">
        <button>Say something</button>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue';
import Component from 'vue-class-component';

import GridRow from './components/gridRow.vue';

@Component({
  components:{
    GridRow
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
div.test-controlls{
  border: 1px solid white;
  height: 10%;
}
</style>
