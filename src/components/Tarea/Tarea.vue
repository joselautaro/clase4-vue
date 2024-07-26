<!-- Configuración dinamica de estilos -->

<!-- Punto 1: Selector de color para el cuadro  -->
<!-- Punto 2: Control deslizante para ajustar el tamaño del cuadro -->
<!-- Punto 3: Cuadro que cambia de color y tamaño basado en valores reactivos -->

<script setup>
import {ref} from 'vue'

const color = ref('#ffffff');

const size = ref(100)


</script>
<template>

    <!-- Selector de color para el cuadro -->
    <label for="color">Color:</label>
    <input type="color" v-model="color">


    <!-- Control deslizante para ajustar el tamaño del cuadro -->
    <label for="size">Tamaño (px):</label>
    <input type="range" id="size" min="50" max="300" v-model="size">

    <!-- Cuadro que cambia de color y tamaño basado en valores reactivos -->
     <div :style="{backgroundColor: color, width: size + 'px', height: size + 'px'}"></div>


</template>

<style scoped>


</style>