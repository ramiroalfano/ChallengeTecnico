<template>
    <div>
    <b-navbar toggleable="lg" type="dark" variant="info">
        <b-navbar-brand href="#">xy</b-navbar-brand>

        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>


        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">
            <b-nav-item @click="register">iniciar sesion</b-nav-item>
            <b-nav-item @click="forgotPassword">Olvidé mi contraseña</b-nav-item>
        </b-navbar-nav>
    </b-navbar>
    </div>
</template>

<script>
export default {
    data() {
        return {
            username: '',
            password: ''
        }
    },
    methods: {
        register() {
            this.username = prompt("Por favor ingresa tu nombre de usuario", "");
            this.password = prompt("Por favor ingresa tu contraseña", "");
            if (this.username != null && this.password != null) {
                // Aquí puedes agregar la lógica para iniciar sesión
                alert(`Usuario ${this.username} ha iniciado sesión con éxito!`);
            }
        },
        forgotPassword() {
            // Aquí puedes agregar la lógica para recuperar la contraseña
            alert('Por favor, comuníquese al 123-456-7890 para recuperar su contraseña.');
        }
    }
}
</script>