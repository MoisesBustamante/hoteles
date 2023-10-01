
<template>
    <div class="mt-9 p-10">
        <div class="container mx-auto">
    <h1 class="text-3xl font-semibold mt-5 mb-3">Editar Hotel</h1>
    <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
      <div>
        <div class="mb-4">
          <label class="block text-gray-700 text-sm font-bold mb-2" for="ciudad">Ciudad:</label>
          <input type="text" id="ciudad" class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline" v-model="hotelEditado.ciudad" required>
        </div>
        <div class="mb-4">
          <label class="block text-gray-700 text-sm font-bold mb-2" for="nombre">Nombre del Hotel:</label>
          <input type="text" id="nombre" class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline" v-model="hotelEditado.nombre" required>
        </div>
        <div class="mb-4">
          <label class="block text-gray-700 text-sm font-bold mb-2" for="nit">NIT:</label>
          <input type="text" id="nit" class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline" v-model="hotelEditado.nit" required>
        </div>
      </div>
      <div>
        <div class="mb-4">
          <label class="block text-gray-700 text-sm font-bold mb-2" for="direccion">Dirección:</label>
          <input type="text" id="direccion" class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline" v-model="hotelEditado.direccion" required>
        </div>
        <div class="mb-4">
          <label class="block text-gray-700 text-sm font-bold mb-2" for="habitaciones">Número máximo de habitaciones:</label>
          <input type="number" id="habitaciones" class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline" v-model="hotelEditado.habitaciones" required>
        </div>
      </div>
    </div>
    <div class="mt-4">
      <a href="/"><button class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded" >Guardar Cambios</button></a>
    </div>
  </div>
</div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        hotelEditado: {
          ciudad: "",
          // Agrega los otros campos aquí y llénalos con los datos del hotel a editar
        }
      };
    },
    methods: {
      guardarCambios() {
        // Envía los datos editados del hotel al backend para su actualización
        // Luego, redirige a la lista de hoteles
      }
    }
  };
  </script>
  