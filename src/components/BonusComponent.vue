<script setup>
import { ref } from 'vue'

// Variable reactiva que controla el color
const esRojo = ref(true)

// Método para cambiar el valor
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