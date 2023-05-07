<template>
    <div>
        <h1>Hello Vue</h1>
        <p>Meu nome é: {{ nome }}</p>
        <MultiplosEventos />
    </div>
</template>

<script>
    import MultiplosEventos from './MultiplosEventos.vue'
    
    export default {
        name: 'PrimeiroComponente',
        data() {
            return {
                nome: 'Davi'

            }
        },
        components: {
            MultiplosEventos
        }
    }
</script>