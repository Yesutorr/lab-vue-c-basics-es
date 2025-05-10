<script setup>
import { ref } from "vue";

const publicaciones = ref([
  {
    titulo: "Introducción",
    descripcion: "Introducción a conceptos",
    contenido: "toda la teoria necesaria para desarrollar la actividad.",
  },
  {
    titulo: "Practica",
    descripcion: "laboratorios y experiencias",
    contenido:
      "Combina lo aprendido en la teoria y pon en practica tus conocimientos.",
  },
  {
    titulo: "Examenes",
    descripcion: "calificaciones y pasantias",
    contenido: "Pon a prueba tus conocimientos y consigue tus objetivos.",
  },
]);
</script>

<template>
  <div>
    <h1>Lista de Publicaciones</h1>
    <div
      v-for="(publicacion, index) in publicaciones"
      :key="index"
      class="post"
    >
      <h2>{{ publicacion.titulo }}</h2>
      <h4>{{ publicacion.descripcion }}</h4>
      <p>{{ publicacion.contenido }}</p>
      <hr />
    </div>
  </div>
</template>

<style>
.post {
  margin-bottom: 1.5rem;
}
</style>
