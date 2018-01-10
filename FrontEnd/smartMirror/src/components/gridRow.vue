<template>
  <div class="grid-row">
    <GridBox/>
    <GridBox/>
    <GridBox/>
  </div>
</template>

<script lang="ts">
import Vue from 'vue';
import Component from 'vue-class-component';

import GridBox from './GridBox.vue';

@Component({
  components:{
    GridBox
  }
})
export default class GridRow extends Vue {
}
</script>

<style>
div.grid-row{
  height: 33%;
  width: 100%;
}
</style>
