<template>
    <div class="tol-sign-up">
        <v-card class="my-16 pa-4">
             <v-toolbar app class="mt-8"
                color="orange"
                height="40px">
                    <v-app-bar-title class="mx-4 my-4">Regístrate</v-app-bar-title>
            </v-toolbar>
            
            <v-text-field class="mt-8" label="Nombre" v-model="nombre" outlined></v-text-field>
            <v-text-field label="Apellidos" v-model="apellidos" outlined></v-text-field>
            <v-text-field label="Email" v-model="emal" outlined></v-text-field>
            <v-text-field label="Dirección" v-model="direccion" outlined></v-text-field>
            <v-text-field label="Localidad" v-model="localidad" outlined></v-text-field>
            <v-text-field label="Contraseña" type="password" v-model="password1" outlined></v-text-field>
            <v-text-field label="Repita contraseña" type="password" v-model="password2" outlined></v-text-field>
            <v-btn color="success" block>Enviar</v-btn>
        </v-card>

    </div>
</template>

<script>
export default{
    layout: 'auth',
    data () {
        return {
            nombre: "",
            apellidos: "",
            email:"",
            direccion: "",
            localidad: "",
            password1: "",
            password2: "",
        }
    }
    
    }
    
</script>

<style scoped>

</style>