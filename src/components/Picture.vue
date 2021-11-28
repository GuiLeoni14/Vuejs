<template>
    <img :src="imagem" :alt="descricao">
</template>
<script>
export default {
    name: 'Picture',
    data() {
        return {
            imagem: '/img/imagem.jpg',
            descricao: 'Guilherme Leoni'
        }
    },
}
</script>