<template>
    <div>
       <h1>motodo de pago</h1>
      <input type=“text” placeholder="numero de tarjeta" v-model="NT" />
    
    <br>
    <br>
    
    <input type=“text” placeholder="nombre de la tarjeta" v-model="nombre" />
   
    <br>
    <br>
     
    <input type=“text” placeholder="cvc" v-model="cvc" />
    <br>
    <br>
    
    <input type=“text” placeholder="expiracion" v-model="expiracion" />
    <br>
    <br>
     

    <h2>
         ---------------------------- <br>   
         numero de tarjeta: {{NT}} <br>
          ---------------------------- <br>
         nombre de la tarjeta: {{nombre}}<br>
          ---------------------------- <br>
         cvc: {{cvc}}<br>
          ---------------------------- <br>
        expiracion: {{expiracion}}<br>
          ---------------------------- <br>
         
         </h2>
   </div> 

    </div>
</template>

<script>

export default {
    name: '',
    data() {
        return {
         

          
      
        }
    }
}
</script>

<style>

</style>
         