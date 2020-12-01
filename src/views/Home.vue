<template>
  <div class="container">
    <div class="card mt-5">
      <div class="card-header text-center">Formulario</div>
      <div class="card-body">
        <form @submit.prevent="procesarFormulario">
          <Formulario :contacto="contacto" />
        </form>
      </div>
    </div>
  </div>
</template>

<script>
import Formulario from '../components/Formulario'
export default {
  name: 'Home',
  components: {
    Formulario
  },
  data(){
    return{
      contacto:{
        nombre:'',
        empresa:'',
        email:'',
        telefono:'',
        mensaje:''
      }
    }
  },
  methods:{
    procesarFormulario(){
      console.log(this.contacto)
    }
  }
}
</script>
