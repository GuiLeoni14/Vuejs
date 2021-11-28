<template>
    <h1>Meu nome é : {{ name }}</h1>
</template>

<script>
export default{
    name: 'LifeCycle',
    data(){
        return{
            name: 'Testando'
        }
    },
    created(){
        this.nome = 'Gui'
    },
    mounted() {
        this.nome = 'Pedro'
    },
}
</script>
