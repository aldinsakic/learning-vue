<script setup>
import { ref } from 'vue'

const text = ref('')

function onInput(e) {
  text.value = e.target.value
}
</script>

<template>
  <input :value="text" @input="onInput" placeholder="Type here">
  <p>{{ text.split('').reverse().join('') }}</p>
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