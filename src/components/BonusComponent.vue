<script setup>
import { ref } from 'vue'


const esRojo = ref(true)


function cambiarColor() {
  esRojo.value = !esRojo.value
}
</script>

<template>
  <div>
    <h2 :style="{ color: esRojo ? 'red' : 'blue' }">
      Este texto cambia de color dinámicamente
    </h2>
    <button @click="cambiarColor">Cambiar Color</button>
  </div>
</template>

<style></style>