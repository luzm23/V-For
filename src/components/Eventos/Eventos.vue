<template>  
    <div class="container">  
      <div class="row mt-4">  
        <div>  
        <h4>Eventos Click</h4>
          <button @click="clic" class="btn btn-danger" type="button">Dale clic</button> 
          <button @click="soybuton" class="btn btn-warning mx-2" type="button">Dale clic 2</button>  
        </div>  
        <div>  
        <h4>Evento Change</h4>  
        <label class="input-group-text" for="">Ingresa tu nombre</label>  
        <input class="form-control mt-2"  type="text" id="nombre" @change="nombreE" /> 
       <p>El nombre ingresado es:  <strong>{{ nombre }}</strong>  </p>
      </div> 
      <div>  
        <h4>Evento Edad</h4>  
        <label class="input-group-text" for="">Ingresa tu Edad</label>  
        <input class="form-control mt-2"  type="text" id="nombre" @change="Edad" /> 
       <p>La edad  ingresado es:  <strong>{{ Edad }}</strong>  </p>
      </div> 

   <div>
    <h3>Eventos Mouse mouseenter y  mouseleave</h3>
      <div class="text-center"
       style="color:#ffff; width:300px; height: 200px; background-color: black; text-align: center; padding: 15px; border-radius: 14px;"   
           @mouseenter="mostrarMensaje" @mouseleave="ocultarMensaje">  
        <p>pase el mouse</p>  
        <p>{{ mensaje }}</p>  
      </div>
      </div>  
      </div>  
    </div>  
  </template>  
  
  <script>  
  export default {  
    data () {  
    return {  
      nombre: '',
      mensaje: '',
    }
    },
    methods: {  
      clic() {  
        alert("Gracias por darle clic");  
      } ,
      soybuton() {  
        alert("Soy un boton");  
      },
      nombreE(event) {  
        this.nombre = event.target.value;  
      },
      mostrarMensaje() {
        this.mensaje = 'el mouse esta dentro del rectangulo'
    },
    ocultarMensaje() {
      this.mensaje = 'el mouse esta fuera del rectangulo'
    },
    Edad(event) {  
      this.Edad = event.target.value;
    }
  } 
  }
  </script>  