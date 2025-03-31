<template>
  <div class="container">
    <h4 class="mt-4 text-center">Horario de Clases de Sistemas Computacioneles</h4>
    <table class="table">
      <thead>
        <tr>
          <th>Hora</th>
          <th>Lunes</th>
          <th>Martes</th>
          <th>Miércoles</th>
          <th>Jueves</th>
          <th>Viernes</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="(h, index) in horario" :key="index">
          <td>{{ h.hora }}</td>
          <td>{{ h.lunes }}</td>
          <td>{{ h.martes}}</td>
          <td>{{ h.miercoles  }}</td>
          <td>{{ h.jueves }}</td>
          <td>{{ h.viernes }}</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script setup>
import { ref } from 'vue';

const horario = ref([
  { hora: '7:00 - 9:00', lunes: 'Programación Lógica y Funcional', martes: 'Inteligencia Artificial', miercoles: 'Desarrollo Ágil', jueves: 'Programación Lógica y Funcional', viernes: '-' },
  { hora: '9:00 - 11:00', lunes: 'Desarrollo Ágil', martes: 'Administración de Redes', miercoles: '-', jueves: 'Administración de Redes', viernes: '-' },
  { hora: '10:00 - 11:00', lunes: '-', martes: '-', miercoles: '-', jueves: '-', viernes: 'Desarrollo Ágil' },
  { hora: '11:00 - 12:00', lunes: '-', martes: '-', miercoles: '-', jueves: '-', viernes: 'Desarrollo En La Nube' },
  { hora: '11:00 - 13:00', lunes: '-', martes: 'Desarrollo En La Nube', miercoles: 'Desarrollo En La Nube', jueves: 'Inteligencia Artificial', viernes: '-' },
  { hora: '13:00 - 14:00', lunes: '-', martes: '-', miercoles: '-', jueves: 'Realidad Aumentada', viernes: '-' },
  { hora: '13:00 - 15:00', lunes: '-', martes: '-', miercoles: 'Realidad Aumentada', jueves: '-', viernes: '-' },
  { hora: '14:00 - 16:00', lunes: '-', martes: '-', miercoles: '-', jueves: '-', viernes: 'Taller De Investigación II' },
  { hora: '15:00 - 17:00', lunes: '-', martes: 'Realidad Aumentada', miercoles: 'Taller De Investigación II', jueves: '-', viernes: '-' }
]);
</script>

<style scoped>
h4 {  
  color: rgb(26, 24, 24);  
  background-color: hsl(7, 26%, 74%);  
  border-radius: 15px;  
  padding: 10px;  
  text-align: center;
} 
.container {
  max-width: 90%;
  margin: 0 auto;
  padding: 20px;
  background-color: #ecd9d9;
  border-radius: 12px;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
}

h3 {
  font-family: 'Arial', sans-serif;
  color: #8f9295;
  font-weight: bold;
  margin-bottom: 20px;
}

.table {
  width: 100%;
  border-collapse: collapse;
  background-color: white;
  border-radius: 8px;
}

.table th, .table td {
  text-align: center;
  padding: 9px 10px;
  font-size: 11px;
  color: #2c3e50;
  border: 1px solid #ddd;
  white-space: nowrap; /* Evita que los textos se vayan a otra línea */
}

.table thead {
  background-color: #3498db;
  color: white;
  text-transform: uppercase;
}

.table tbody tr:nth-child(odd) {
  background-color: #f0f4f7;
}

.table tbody tr:hover {
  background-color: #ecf0f1;
}
</style>
