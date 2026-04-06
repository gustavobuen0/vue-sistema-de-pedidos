<template>
    <h1>Meu nome é: {{ nome }}</h1>
</template>

<script>
export default {
    name: 'LifeCycle',
    data() {
        return {
            nome: 'Ainda não sei',
        }
    },
    created() {
        setTimeout(() => {
            this.nome = "Gustavo";
        }, 5000);
    },
    mounted() {
         setTimeout(() => {
            this.nome = "Gabriel";
        }, 8000);
    }
}
</script>