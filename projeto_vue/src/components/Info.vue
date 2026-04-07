<template>
    <div>
        <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
        <p v-else>Estou em Busca de Novas Oportunidades.</p>
        <p>Formado em Gestão da Tecnologia da Informação pela FATEC - Itaquaquecetuba</p>
        <p>Pós Graduando em Segurança da Informação pela PUC Campinas em parceria com a PUC Paraná</p>

        <p v-if="4 > 2">Testando</p>

        <p v-show="mostrar_email">Mande uma mensagem para {{ email }}</p>
    </div>
</template>

<script>
export default {
    name: 'Info',
    data () {
        return {
            esta_trabalhando: false,
            mostrar_email: true,
            email: 'gustavobuenoctt@gmail.com'
        }
    }
}
</script>