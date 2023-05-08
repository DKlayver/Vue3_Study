<template>
    <div>
        <Header :esta_logado="true" />
        <PrimeiroComponente />
        <p>O dado do app é: {{ testando }}</p>
        <LifeCycle />
        <Pessoa />
    </div>
</template>

<script>
    import Header from "./components/Header.vue"
    import PrimeiroComponente from "./components/PrimeiroCOmponente.vue";
    import LifeCycle from "./components/LifeCycle.vue";
    import Pessoa from "./components/Pessoa.vue";
    
    export default {
        name:'App',
        components: {
            Header,
            PrimeiroComponente,
            LifeCycle,
            Pessoa

         },
         data() {
            return{
                testando: "teste"
            }
         }
    }
</script>

<style>
    body {
        background-color: #333;
        color: #FFF;
    }
    a {
        color: rgb(42, 115, 252)
    }
</style>