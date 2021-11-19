<template>
    <div class="tol-sign-in">
        <v-card class="my-16">
             <v-toolbar app class="mt-8"
                color="orange"
                height="40px">
                    <v-app-bar-title class="mx-4 my-4">Mi Cuenta</v-app-bar-title>
            </v-toolbar>
            
            <v-text-field class="mt-8" placeholder="email" outlined></v-text-field>
            <v-text-field placeholder="password" type="password" outlined></v-text-field>
            <v-btn color="success" block>Submit</v-btn>
        </v-card>

    </div>
</template>

<script>
export default{
    layout: 'auth',
    
    }
    
</script>

<style scoped>

</style>