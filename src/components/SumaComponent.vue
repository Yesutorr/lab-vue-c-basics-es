<script setup>
import { ref } from 'vue';

const numero1 = ref(2)
const numero2 = ref(2)

function mostrarResultado() {
  return `El resultado de ${numero1.value} + ${numero2.value} es ${numero1.value + numero2.value}`
}

</script>

<template>
 <div>
    {{ mostrarResultado() }}
  </div>
   
 </template>

<style>

</style>