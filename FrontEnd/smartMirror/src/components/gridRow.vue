<template>
  <div class="grid-row">
    <span v-show="!isCommunicationRow || (isCommunicationRow && !communicationActive)">
    <GridBox/>
    <GridBox/>
    <GridBox/>
    </span>
    <span v-show="isCommunicationRow && communicationActive">
      <p class="message">{{message}}</p>
    </span>
  </div>
</template>

<script lang="ts">
import Vue from 'vue';
import {Component, Prop} from 'vue-property-decorator';

import GridBox from './GridBox.vue';

@Component({
  components:{
    GridBox
  }
})
export default class GridRow extends Vue {
  @Prop()
  public isCommunicationRow:boolean;

  private communicationActive:boolean = false;
  private message:string = "Hello";
}
</script>

<style>
div.grid-row{
  height: 33%;
  width: 100%;
  overflow: hidden;
}

p.message{
  margin-top:10%;
  font-size: 5em;
  color:white;
}
</style>
