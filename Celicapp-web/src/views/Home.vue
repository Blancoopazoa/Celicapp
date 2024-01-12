<template>
    <div>
      <h1 class="text-2xl font-bold mb-4">Bienvenido a CelicApp</h1>
      <Login />
    </div>
  </template>
  
  <script>
  import Login from '../components/Login.vue';
  
  export default {
    components: {
      Login,
    },
  };
  </script>