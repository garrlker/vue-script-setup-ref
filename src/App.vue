<template>
  <HelloWorld ref="hwref"/>
</template>

<script setup>
import { onMounted, ref } from 'vue'
import HelloWorld from './components/HelloWorld.vue'

const hwref = ref();

onMounted(() => {
  console.log(hwref.value);
})
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>