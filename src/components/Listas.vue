<script>
export default {
  data() {
    return {
      alumnos: [
        { nc: 12345, nombre_completo: 'Yanet González García', gustos: 'Escuchar música y Comer' },
        { nc: 12346, nombre_completo: 'Susana Gómez Martínez', gustos: 'Música y Leer' },
        { nc: 12347, nombre_completo: 'Edgar Ramírez Torres', gustos: 'Jugar videojuegos y Programar' },
        { nc: 12348, nombre_completo: 'Aldair Hernández Ruiz', gustos: 'Fútbol y Ver series' },
        { nc: 12349, nombre_completo: 'Carlos Mendoza Ruiz', gustos: 'Escalar montañas' },
        { nc: 12350, nombre_completo: 'Ana Chávez Domínguez', gustos: 'Fotografía y Pintar' },
        { nc: 12351, nombre_completo: 'Roberto Díaz Hernández', gustos: 'Cocinar y Correr' },
        { nc: 12352, nombre_completo: 'Fernanda López Pérez', gustos: 'Bailar y Viajar' },
        { nc: 12353, nombre_completo: 'Jorge Ramírez Salazar', gustos: 'Tocar la guitarra y Natación' },
        { nc: 12354, nombre_completo: 'Diana Torres Muñoz', gustos: 'Ver series y Dibujar' }
      ]
    };
  }
}
</script>

<template>
  <div class="container">
    <h3 class="title mt-4">LISTA DE ALUMNOS</h3>
    <ul>
      <li v-for="alumno in alumnos" :key="alumno.nc">
        <p><strong>ID:</strong> {{ alumno.nc }}</p>
        <p><strong>Nombre:</strong> {{ alumno.nombre_completo }}</p>
        <p><strong>Gustos:</strong> {{ alumno.gustos }}</p>
      </li>
    </ul>
  </div>
</template>

<style>
body {
  background-color: #0d1b2a;
  font-family: Arial, sans-serif;
}

.title {
  color: #f4a261;
  background-color: #1b263b;
  border-radius: 15px;
  padding: 15px;
  text-align: center;
  margin-top: 20px; 
}

ul {
  list-style-type: none;
  padding: 0;
  margin-left: 0;
}

li {
  background: linear-gradient(135deg, #1b263b, #415a77);
  color: white;
  border-radius: 15px;
  padding: 15px;
  margin: 10px 0;
  box-shadow: 3px 3px 10px rgba(0, 0, 0, 0.2);
  text-align: left; 
}

p {
  margin: 5px 0;
  text-align: left; 
}

strong {
  color: #f4a261;
}
</style>