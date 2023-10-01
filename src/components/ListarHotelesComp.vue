<script setup>
import { onMounted } from 'vue'
import { initFlowbite } from 'flowbite'

// initialize components based on data attribute selectors
onMounted(() => {
  initFlowbite()
})
</script>
<template>
 <div class="mt-9 p-10">
  <div class="relative overflow-x-auto border shadow-md sm:rounded-lg">
    <table class="w-full text-sm text-left text-blue-100 dark:text-blue-100">
      <thead class="text-xs text-white uppercase bg-blue-600 dark:text-white">
        <tr>
          <th scope="col" class="px-6 py-3">
            Ciudad
          </th>
          <th scope="col" class="px-6 py-3">
            Nombre del Hotel
          </th>
          <th scope="col" class="px-6 py-3">
            NIT
          </th>
          <th scope="col" class="px-6 py-3">
            Dirección
          </th>
          <th scope="col" class="px-6 py-3">
            Número Máximo de Habitaciones
          </th>
          <th scope="col" class="px-6 py-3">
            Acción
          </th>
        </tr>
      </thead>
      <tbody>
        <tr class="bg-blue-500 border-b border-blue-400">
          <td class="px-6 py-4 font-medium text-blue-50 whitespace-nowrap dark:text-blue-100">
            Ciudad 1
          </td>
          <td class="px-6 py-4">
            Emperador
          </td>
          <td class="px-6 py-4">
            123456789
          </td>
          <td class="px-6 py-4">
            calle 15
          </td>
          <td class="px-6 py-4">
            100
          </td>
          <td class="px-6 py-4">
            <a href="/detalle" class="font-medium text-white hover:underline">
              <i class="fas fa-eye"></i>               
              <font-awesome-icon icon="fa-solid fa-eye" />
            </a>
            <a href="/edit" class="font-medium text-white hover:underline ml-2">
              <i class="fas fa-edit"></i> 
              <font-awesome-icon icon="fa-solid fa-pen-to-square" />
            </a>
            <a @click="showAlert" class="font-medium text-white hover:underline ml-2">
              <i class="fas fa-trash"></i> <!-- Icono de basura para "Eliminar" -->
              <font-awesome-icon icon="fa-solid fa-trash" />
            </a>
          </td>
        </tr>
        <tr class="bg-blue-500 border-b border-blue-400">
          <td class="px-6 py-4 font-medium text-blue-50 whitespace-nowrap dark:text-blue-100">
            Sahagun
          </td>
          <td class="px-6 py-4">
            Foreman
          </td>
          <td class="px-6 py-4">
            987654321
          </td>
          <td class="px-6 py-4">
            troncal Occidente
          </td>
          <td class="px-6 py-4">
            150
          </td>
          <td class="px-6 py-4">
            <a href="/detalle" class="font-medium text-white hover:underline">
              <i class="fas fa-eye"></i> <!-- Icono de ojo para "Ver" -->
              <font-awesome-icon icon="fa-solid fa-eye" />
            </a>
            <a href="/edit" class="font-medium text-white hover:underline ml-2">
              <i class="fas fa-edit"></i> 
              <font-awesome-icon icon="fa-solid fa-pen-to-square" />
            </a>
            <a @click="showAlert" class="font-medium text-white hover:underline ml-2">
              <i class="fas fa-trash"></i> 
              <font-awesome-icon icon="fa-solid fa-trash" />
            </a>
          </td>
        </tr>
        <!-- Puedes agregar más filas con datos aquí -->
      </tbody>
    </table>
    <a href="/about"><button  type="button"  class="text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm px-4 py-2 text-center mr-3 md:mr-0 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800 m-4 p-4">Crear Hotel</button></a>
    
  </div>
</div>


  </template>
  <script>
    export default {
    name:'SweetAlert2',
    methods: {
      
      showAlert() {
      
      this.$swal('Desea eliminar este hotel?');
    },
    }
  }
</script>
  
  
  
  

  

  