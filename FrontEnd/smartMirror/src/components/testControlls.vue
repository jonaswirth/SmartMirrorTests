<template>
  <div class="test-controlls">
      <button>Say something</button>
  </div>
</template>

<script lang="ts">
import Vue from 'vue';
import {Component} from 'vue-property-decorator';

@Component
export default class TestControlls extends Vue{

}

</script>

<style>
div.test-controlls{
  border: 1px solid white;
  height: 10%;
}
</style>
