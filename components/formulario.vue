<template>
  <div >
    <div v-if="mostrar2 == true  ">
      <h1>FORMULARIO DE ENTREGA</h1>
      
    <input type=“text” placeholder="nombre" v-model="nombre" />
    
    <br>
    <br>
    
    <input type=“text” placeholder="apellido" v-model="apellido" />
   
    <br>
    <br>
     
    <input type=“text” placeholder="ciudad" v-model="ciudad" />
    <br>
    <br>
    
    <input type=“text” placeholder="sexo" v-model="sexo" />
    <br>
    <br>
     
   <input type=“text” placeholder="fecha de nacimiento" v-model="fecha" />
    <br>
    <br>
     
    <input type=“text” placeholder="direccion de entrega" v-model="direccion" />
    <br> <br>

    <button type="primary" @click="mostrarmas = true"> mostrar datos</button>
    <button type="primary" @click="mostrarmas = false"> ocultar datos</button>
    
    <div  v-if="mostrarmas == true  ">
         <h1>datos de cliente</h1>
         
         <h2>
         ---------------------------- <br>   
         nombre: {{nombre}} <br>
          ---------------------------- <br>
         apellido: {{apellido}}<br>
          ---------------------------- <br>
         ciudad: {{ciudad}}<br>
          ---------------------------- <br>
         sexo: {{sexo}}<br>
          ---------------------------- <br>
         fecha: {{fecha}}<br>
          ---------------------------- <br>
         direccion: {{direccion}}<br>
         ---------------------------- 
         </h2>
    </div>
        <button type="primary" @click="mostrar2 = false"> formulario de proveedores</button>
   </div>

   <div v-if="mostrar2 == false  ">

     <h1>formulario de proveedores</h1>
      <input type=“text” placeholder="titulo" v-model="titulo" />
    
    <br>
    <br>
    
    <input type=“text” placeholder="capital" v-model="capital" />
   
    <br>
    <br>
     
    <input type=“text” placeholder="ubicacion" v-model="ubicacion" />
    <br>
    <br>
    
    <input type=“text” placeholder="tiempo de entrega" v-model="tiempo" />
    <br>
    <br>
     
   <input type=“text” placeholder="fecha de ingreso" v-model="fecha" />
    <br>
    <br>
     
    <input type=“text” placeholder="tipo de entrega" v-model="tipo" />
    <br> <br>

    <input type=“text” placeholder="lista de productos" v-model="productos" />
    <br> <br>

    <h2>
         ---------------------------- <br>   
         titulo: {{titulo}} <br>
          ---------------------------- <br>
         capital: {{capital}}<br>
          ---------------------------- <br>
         ubicacion: {{ubicacion}}<br>
          ---------------------------- <br>
         tiempo de entrega: {{tiempo}}<br>
          ---------------------------- <br>
         fecha de ingreso: {{fecha}}<br>
          ---------------------------- <br>
         tipo de entrega: {{tipo}}<br>
         ---------------------------- 
          <br>
         lista de productos: {{productos}}
         </h2>
   </div>

  </div>
</template>

<script>
export default {
  name:'',
  data () {
    return {
        mostrarmas: false,
        mostrar2: true,
        mostrar:true,
        nombre: null,
        apellido: null,
        ciudad: null,
        sexo: null,
        fecha: null,
        direccion: null,
        productos: null, 
    }
  },
  methods:{
      onclick:function(){
          console.log(this.nombre)
          console.log(this.apellido)
      }
  }
}
</script>

<style>
</style>