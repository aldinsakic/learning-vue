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
  input{
    height: 50px;
    width: 100%;
    font-size: 24pt;
    text-align: center;
    background: rgb(186,102,186);
    background: linear-gradient(90deg, rgba(186,102,186,1) 0%, rgba(0,0,0,1) 80%);
    border: none;
    color: var(--color-text);
  }
</style>