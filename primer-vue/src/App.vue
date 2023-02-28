<script setup>
  const name = 'Vue Dinamico'
  const styleColor = 'color: blue'
  const arrayValues=['valor 1', 'valor 2', 'valor 3']
  const activo = true
</script>

<template>
  <h1>Hola {{ name }}</h1>
  <!-- V-bind -->
  <h2 v-bind:style="styleColor">Soy azul</h2>
  <!-- v bind con : -->
  <h2 :style="styleColor">Soy azul</h2>
  <!--
    Usar algunas cosas de JS dentro de los corchetes
  -->
  <h3>{{ name.toUpperCase() }}</h3>
  <h3>{{ arrayValues }}</h3>
  <h3> {{ activo ? 'Activo': 'Inactivo' }}</h3>
  

</template>

<style>
h1 {
  color: red;
}
</style>