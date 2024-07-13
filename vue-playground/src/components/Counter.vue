<script setup>
import { ref } from 'vue'

const count = ref(0)

function increment(){
  count.value++
}
</script>

<template>
  <button class="pinkBg" @click="increment">{{ count }}</button>
</template>

<style scoped>
  button{
    border: none;
    width: 150px;
    height: 50px;
    font-family: Arial, Helvetica, sans-serif;
    font-size: 24pt;
    color: var(--color-text);
  }
</style>