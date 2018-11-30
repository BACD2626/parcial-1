<template>
  <div id="app" >
    
     <div  v-if="mostrar == true  ">
          
            <h1>INICIA SECION</h1>
            <input type=“text” placeholder="usuario" v-model="user" /><br> <br>
          
            <input type=“text” placeholder="pass" v-model="pass" /><br> <br>
            

            <button type="primary" @click="mostrar = false"> login</button>
          
      
     
     </div>

      <div v-if="mostrar == false  " >
        
     <formulario/>
     <br><br>
     <button type="primary" @click="mostrar = true"> salir</button>
     <button type="primary" @click="mostrarr = true"> pago</button>
    </div>
        <div v-if="mostrarr == true  ">
          <pago/>
        </div>
  </div>
</template>

<script>
import pago from'./components/pago.vue'
import formulario from './components/formulario.vue'
export default {
  name: 'app',
  components:{
     formulario, pago
  },
  data () {
    
    
    return {
      
      mostrar: true,
      mostrarr: false,
      
      
    }
  }
}
</script>

<style>

</style>