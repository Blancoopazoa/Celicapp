<template>
    <div class="min-h-screen flex items-center justify-center">
    <form class="bg-white shadow-md rounded px-8 pt-6 pb-8 mb-4 w-full max-w-md flex items-center justify-center">
      <div class="text-body">
      <div class="mb-6">
        <label class="block text-gray-700 text-sm font-bold mb-2" for="username">
          Usuario
        </label>
        <input v-model="username" class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline" id="username" type="text" placeholder="Ingrese su usuario">
      </div>
      <div class="mb-6">
        <label class="block text-gray-700 text-sm font-bold mb-2" for="password">
          Contraseña
        </label>
        <input v-model="password" class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline" id="password" type="password" placeholder="********">
      </div>
      <div class="flex items-center justify-center">
        <button class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded focus:outline-none focus:shadow-outline" type="submit">
          Iniciar Sesión
        </button>
      </div>
      </div>
    </form>
  </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        username: '',
        password: '',
      };
    },
    methods: {
      login() {
        if (this.username === 'usuario' && this.password === 'contraseña') {
          alert('Inicio de sesión exitoso');
        } else {
          alert('Error en el inicio de sesión. Usuario o contraseña incorrectos.');
        }
      },
    },
  };
  </script>
  
  <style scoped>
  .text-body{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
  }
  </style>
  