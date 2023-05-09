<template>
    <div>
        <img :src="avatar" :alt="descricao" width="240"> 
        <MudarImagem @mudarImagem="trocarImagem" />
    </div>
</template>
<script>
import MudarImagem from "./MudarImagem.vue";

export default {
    name: "Picture",
    data() {
        return {
            avatar: "/img/programmer.png",
            descricao: "Davi Klayver"
        };
    },
    components: { 
        MudarImagem 
    },
    methods: {
        trocarImagem() {
            console.log("aaaa"),
            this.avatar = '/img/programmer2.png';
        }
    }
}
</script>