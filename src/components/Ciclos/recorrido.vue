<script>  
export default {  
  data() {  
    return {  
      // Datos de alumnos con ID, nombre completo, carrera y email  
      alumnos: [  
        { id: 1, nombreCompleto: 'Luz Maria Mendoza Cortes', carrera: 'ISC', email: 'luzh@gmail.com' },  
        { id: 2, nombreCompleto: 'Jose Luis Mendoza Cortes', carrera: 'TICS', email: 'jose@gmail.com' },  
        { id: 3, nombreCompleto: 'Aurora Cortes Lopez',      carrera: 'ISC', email: 'auroram@gmail.com' },  
        { id: 4, nombreCompleto: 'Ana Pérez León',          carrera: 'TI',   email: 'anap@gmail.com' },  
        { id: 5, nombreCompleto: 'Juliana Pérez Hernández', carrera: 'TI',  email: 'juliana@gmail.com' },  
        { id: 6, nombreCompleto: 'Yessica López Jiménez',   carrera: 'TI',  email: 'yesica@gmail.com' },  
        { id: 7, nombreCompleto: 'Alicia Mendoza Ramírez',  carrera: 'TI',  email: 'alicia@gmail.com' }  
      ]  
    }  
  }  
}  
</script>  

<template>  
  <div class="container">  
    <h3 class="mt-4">Lista de alumnos</h3>  
    <ul>  
      <li v-for="alumno in alumnos" :key="alumno.id">  
        <strong>ID:</strong> {{ alumno.id }} |  
        <strong>Nombre:</strong> {{ alumno.nombreCompleto }} |  
        <strong>Carrera:</strong> {{ alumno.carrera }} |  
        <strong>Email:</strong> {{ alumno.email }}  
      </li>  
    </ul>  
  </div>  
</template>   

<style>  
h3 {  
  color: rgb(26, 24, 24);  
  background-color: hsl(7, 26%, 74%);  
  border-radius: 15px;  
  padding: 10px;  
  text-align: center;
}  

ul {  
  list-style-type: none;  
  padding: 0;  
}  

li {  
  color: white;  
  background-color: black;  
  border-radius: 15px;  
  padding: 10px;  
  margin: 10px;  
  text-align: left;  
  display: flex;  
  justify-content: space-between;  
  flex-wrap: wrap;  
}  
</style>  
