<template>
  <div class="grid-box">
  </div>
</template>

<script lang="ts">
import Vue from 'vue';
import Component from 'vue-class-component';

@Component
export default class GridBox extends Vue {
}
</script>

<style>
div.grid-box{
  height: 93%;
  width: 31%;
  border: 1px solid white;
  margin: 1%;
  float: left;
  border-radius: 7px;
}
</style>
