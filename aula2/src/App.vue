<template>
    <PrimeiroComponente />
</template>

<script>
    import PrimeiroComponente from "./components/PrimeiroCOmponente.vue";
    import LifeCycle from "./components/LifeCycle.vue";
    export default {
        name:'App',
        components: {
            PrimeiroComponente,
            LifeCycle,
         }
    }
</script>