<template>
    <div class="finalizar">
        <h1>Finalizar compra</h1>
        <v-container>
            <v-row class="fila-1">
                <v-btn color="rgb(0,150,100)"><nuxt-link to="/signUp" class="liso">Registrarse</nuxt-link></v-btn>
                <v-btn color="blue"><nuxt-link to="/signIn" class="liso">Mi cuenta</nuxt-link></v-btn> 
            </v-row>
            <v-row>
                <div class="externo">
                    <div class="interno">
                        <p class="par">Necesitamos tus datos para procesar tu pedido</p>
                    </div>
                </div>
            </v-row>
            <v-row>
                <v-col cols=2></v-col>
                <v-col cols=8>
                    <div class="frontal">
                        <h3 class="cabeza">TOTAL ........XXXX €</h3>
                        <p style="margin-top: 50px;">NOTA: Aquí reservaríamos un espacio para introducir el IVA , transporte o cualquier otro concepto que nos parezca interesante</p>
                        <v-btn style="margin-top: 150px;" color="primary">Aceptar</v-btn>
                    </div>
                </v-col>
                <v-col cols=2></v-col>
            </v-row>
        </v-container>    
    </div>
</template>
<style scoped>
.fila-1 {
    display: flex;
    justify-content: space-between;
    margin-bottom: 40px;
}
.par {
    width: 200px;

}
.externo {
    background-color: yellow;
    width: 200px;
    height: 65px;
    padding: 10px;
    margin-top: -30px;
}
.interno {
   background-color: rgba(0,0,0,.3);
   padding-left: 5px;
}
.frontal {
    height: 400px;
   
    border-radius: 25px;
    box-shadow: 5px 5px 10px;
    margin-bottom: 50px;
    padding: 30px;
}
.cabeza {
    display: flex;
    justify-content: center;
    margin-top: 20px;
}
.liso {
    color: black;
    text-decoration: none;
}
</style>

