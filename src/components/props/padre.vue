<script setup>  
import { ref } from 'vue' 
import Hijo1 from './Hijo1.vue';
import Hijo2 from './Hijo2.vue';

</script>  

<style>  
/* Agrega aquí estilos CSS si es necesario */  
</style>  

<template> 
<div class="container">
<h1>Soy el componente</h1>
<Hijo1 class="mt-4" edad ="10"/> 
<Hijo2 class="mt-4" edad = "4"/> 
</div> 
</template> 
<style scoped></style> 

