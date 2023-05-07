<template>
    <h1>Meu nome é: {{ nome }}</h1>
</template>

<script>
    export default {
        name: 'LifeCycle',
        data() {
            return {
                nome: 'Ainda nao sei',
            }
        },
        created() {
            setTimeout(() => {
                this.nome = 'Davi'
            }, 1000);

            this.lifeCycle()
        },
        mounted() {
            setTimeout(() => {
                this.nome = 'Klayver'               
            }, 2000);
           
            this.lifeCycle() 
        },
        methods: {
            lifeCycle() {
                console.log("Executou");
            }
        }
    }

</script>