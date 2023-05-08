<template>
    <div>
        <h1>Hello Vue</h1>
        <p>Meu nome é: {{ nome }}</p>
        <MultiplosEventos />
        <Reutilizacao />
        <Reutilizacao />
        <Reutilizacao />
        <Reutilizacao />
    </div>
</template>

<script>
    import Reutilizacao from './Reutilizacao.vue';
    import MultiplosEventos from './MultiplosEventos.vue'

    export default {
        name: 'PrimeiroComponente',
        data() {
            return {
                nome: 'Davi'

            }
        },
        components: {
            MultiplosEventos,
            Reutilizacao
        }
    }
</script>