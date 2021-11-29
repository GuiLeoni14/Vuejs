<template>
    <div>
        <img :src="imagem" :alt="descricao">
        <MudarImagem @mudar-imagem="trocarImagem" />
    </div>
</template>
<script>
import MudarImagem from "./MudarImagem.vue"
export default {
    name: 'Picture',
    components:{
        MudarImagem,
    },
    methods: {
        trocarImagem(){
            this.imagem = "/img/download.jpg"
        }
    },
    data() {
        return {
            imagem: '/img/imagem.jpg',
            descricao: 'Guilherme Leoni'
        }
    },
}
</script>