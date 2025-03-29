<script setup>  
import { ref } from 'vue'  
defineProps
({
  edad:String
})

</script>  

<style>  
/* Agrega aquí estilos CSS si es necesario */  
</style>  

<template>  
  <h6>Soy el componente hijo 2</h6>
  <p>{{ edad }}</p>
</template> 
<style scoped></style> 

