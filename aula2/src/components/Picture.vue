<template>
    <img :src="avatar" :alt="descricao" width="240">
</template>
<script>
export default {
    name: 'Picture',
    data() {
        return {
        avatar: "/img/programmer.png",
        descricao: "Davi Klayver"
        }
    }
}
</script>