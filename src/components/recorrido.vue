<script>
export default {
  data() {
    return {
      // DATOS DE ALUMNOS
      alumnos: [
        { nc: 12345, nombre: 'Yanet', carrera: 'ISC' },
        { nc: 12345, nombre: 'Susana', carrera: 'TICS' },
        { nc: 12345, nombre: 'Edgar', carrera: 'ISC' },
        { nc: 12345, nombre: 'Aldair', carrera: 'TICS' },
      ]
    };
  }
}
</script>
<template>
    <div class="container">
      <h3 class="mt-4 text-center">Lista de alumnos</h3>
      <ul>
        <li v-for="alumno in alumnos" :key="alumno.nc">
          <strong>{{ alumno.nombre }}</strong> - 
          <strong>{{ alumno.carrera }}</strong>
        </li>
      </ul>
    </div>
  </template>
  
<style>
h3 {
    color: black;
    background-color: rgb(225, 211, 147);
    border-radius: 15px;
    padding: 10px;
}
ul {
  list-style-type: none;
  padding: 0%;
}

li {
  color: white;
  background-color: black;
  border-radius: 15px;
  padding: 10px;
  margin: 10px;
  text-align: center;
}
</style>