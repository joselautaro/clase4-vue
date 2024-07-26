<script setup>

import {defineProps} from 'vue';

// Primero se define la constante, despues se le asigna el nombre y luego como las props son funciones, llevan dentro un objeto

const props = defineProps({
    // Ejemplo 1
    title: String,

    // Ejemplo 2
    isAuthenticated: Boolean,

    // Ejemplo3
    userInfo: Object,

    // Ejemplo 4
    items: Array,

    // Ejemplo 5
    tableConfig: Object,

    // Ejemplo 6
    onClick: Function
})

</script>

<template>
    <!-- Ejemplo 1 -->

    <!-- <div>
        <h2>{{ title }}</h2>
    </div> -->

    <!-- Ejemplo 2 -->
     <!-- <div v-if="isAuthenticated">
        Usuario autenticado
     </div>
     <div v-else>
        Usuario no autenticado
     </div> -->

     <!-- Ejemplo 3 -->
     <!-- <div>
        <h3>{{ userInfo.nombre }}</h3>
        <p>{{ userInfo.edad }}</p>
     </div> -->

     <!-- Ejemplo 4 -->

     <!-- <ul>
        <li v-for="(item, index) in items" :key="index"> {{ item }} </li>
     </ul> -->

     <!-- Ejemplo 5 -->
     <!-- <table>
        <thead>
            <tr>
                <th v-for="(col, index) in tableConfig.columns" :key="index"> {{ col }} </th>
            </tr>
        </thead>
        <tbody>
            <tr v-for="(row, index) in tableConfig.data" :key="index">
                <td>{{ row.name }}</td>
                <td>{{ row.age }}</td>
            </tr>
        </tbody>
     </table> -->

     <!-- Ejemplo 6 -->
     <button @click="onClick">Clickeame!</button>


  
</template>

<style scoped>

</style>