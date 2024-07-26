<script setup>

import Hijo from '@/components/Hijo/Hijo.vue'

//   const tableConfig = {
//     columns: ["Name", "Age"],
//     sorteable: true,
//     data: [
//       { name: "Alberto", age: 18 },
//       { name: "Maria", age: 20 },
//       { name: "Antonio", age: 20 },
//     ],
// };

const handleClick = () =>{
    alert('Me has clickeado!')
}

</script>

<template>
    <!-- Ejemplo 1 -->
    <!-- <Hijo title="Bienvenidos"></Hijo> -->
    
    <!-- Ejemplo 2 -->
    <!-- <Hijo :isAuthenticated="false"></Hijo> -->

    <!-- Ejemplo 3 -->
     <!-- <Hijo :userInfo="{nombre: 'Alberto', edad: 30}"></Hijo> -->

     <!-- Ejemplo 4 -->

     <!-- <Hijo :items="['Item 1', 'Item 2', 'Item 3']"></Hijo> -->


     <!-- Ejemplo 5 -->
     <!-- <Hijo :tableConfig="tableConfig"></Hijo> -->

     <!-- Ejemplo 6 -->
     <Hijo :onclick="handleClick"></Hijo>

  
</template>

<style scoped>

</style>