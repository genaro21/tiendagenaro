<template>
    <div class="tol-carrito">
        <v-container class="mb-10">
            <h1>Carrito</h1>
            <v-row class="fila-1">
                <v-col cols="1"></v-col>
                <v-col cols="4" class="c1">
                    <p class="d-flex justify-center"><u>Artículo</u></p>
                </v-col>
                <v-col cols="1" class="c2">
                    <p class="d-flex justify-center"><u>Cantidad</u></p>
                </v-col>
                <v-col cols="1" class="c3">
                    <p class="d-flex justify-center"><u>Importe</u></p>
                </v-col>
                <v-col cols="4" class="c4">
                    <p class="d-flex justify-center"><u>Suma Total</u></p>
                </v-col>
                <v-col cols="1"></v-col>
            </v-row> 
            <v-row class="fila-2"> 
                <v-btn color="rgb(0,150,100)" @click="onClick">Volver a tienda</v-btn>
                <v-btn color="blue"><nuxt-link to="/finalizar_compra" class="liso">Finalizar compra</nuxt-link></v-btn>
            </v-row>      
        </v-container>    
    </div>
</template>

<script>
export default{
    methods: {
        onClick () {
            const prePage = this.$route.query.prePage
            if (prePage) {
                this.$router.push('/'+ prePage)
            } else {
                this.$router.push('/home')
            }
        }
    }
}    
</script>

<style scoped>
.c1 {
    background-color: rgb(225,225,225);
    border-radius: 50px 0px 0px 50px;
}
.c2 {
    background-color: rgb(225,225,225);
}
.c3 {
    background-color: rgb(225,225,225);
} 
.c4 {
    background-color: rgb(225,225,225);
    border-left: 3px solid black;
    border-radius: 0px 50px 50px 0px;
} 
.fila-1 {
    height: 400px;
} 
.fila-2 {
    display: flex;
    justify-content: space-around;
    margin-top: 50px;
    margin-bottom: 10px;

}
.liso {
    color: black;
    text-decoration: none;
}

</style>
