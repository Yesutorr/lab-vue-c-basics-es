<script setup>
import { ref } from 'vue';
const printTrue = ref(true)
</script>

<template>
<div>
    <p v-if="printTrue">Esto se imprime porque la condicion es true</p>
    <p v-else> La condición es false </p>
</div>
</template>

<style>
</style>