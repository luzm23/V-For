<script setup>  
import { ref } from 'vue'  

const bienvenida = ref("Bienvenidos a la seccion de condicionales")  
const nombre = ref("Luz Maria")  
const apellidos = ref("Mendoza Cortes")  
</script>  

<style>  
/* Agrega aquí estilos CSS si es necesario */  
</style>  

<template>  
  <div class="container">  
    <h2 class="text-center">{{ bienvenida }}</h2>  
    <div class="row">  
      <div class="col-md-6">  
        <h6>{{ nombre }}</h6>  
        <h6>{{ apellidos }}</h6>  
      </div>  
    </div>  
  </div>  
</template>  

