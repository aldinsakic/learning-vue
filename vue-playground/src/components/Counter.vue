<script setup>
import { ref } from 'vue'

const count = ref(0)

function increment(){
  count.value++
}
</script>

<template>
  <button @click="increment">{{ count }}</button>
</template>

<style scoped>
  button{
    background-color: #ba66ba;
    border: none;
    border-radius: 50%;
    width: 50px;
    height: 50px;
    font-family: Arial, Helvetica, sans-serif;
    font-size: x-large;
  }
</style>