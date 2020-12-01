<template>
<div class="container">


      <div class="form-row">
            <div class="form-group col-md-6">
            <label for="nombre">Nombre</label>
            <input type="text" class="form-control" id="nombre" v-model="contacto.nombre">
            </div>
            <div class="form-group col-md-6">
            <label for="empresa">Empresa</label>
            <input type="text" class="form-control" id="empresa" v-model="contacto.empresa">
            </div>
        </div>
        <div class="form-row">
            <div class="form-group col-md-6">
            <label for="inputEmail4">Email</label>
            <input type="email" class="form-control" id="inputEmail4" v-model="contacto.email">
            </div>
            <div class="form-group col-md-6">
            <label for="telefono">Telefono</label>
            <input type="number" class="form-control" id="telefono" v-model="contacto.telefono">
            </div>
        </div>
        <div class="form-row">
            <div class="form-group col-md-12">
            <label for="mensaje">Mensaje</label>
            <textarea class="form-control" id="mensaje" cols="30" rows="10" v-model="contacto.mensaje"></textarea>
            </div>
        </div>

        <button type="submit" class="btn btn-primary btn-sm btn-block">Enviar</button>
</div>
</template>

<script>
    export default {
        props:{
            contacto:Object
        }
        
    }
</script>
