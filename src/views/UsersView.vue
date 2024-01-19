<template>
    <div>
        {{ $route.params.id }} - usuário
        <br>
        <button @click="login">Entrar</button>
    </div>
</template>

<script>
    export default {
        created() {
            console.log(this.$route);
        },
        methods : {
            login () {
                this.$router.push('/about');
                console.log("Login...");
            }
        }
    }
</script>