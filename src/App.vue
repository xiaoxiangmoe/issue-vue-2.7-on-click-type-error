<script setup lang="ts">
import HelloWorld from './HelloWorld.vue';

const handleClick = (event: MouseEvent) => {
  console.log(event);
};
 
</script>

<template>
  <div id="app">
    <HelloWorld @click="handleClick" />
  </div>
</template>
