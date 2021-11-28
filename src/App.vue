<template>
    <div>
        <Header/>
        <PrimeiroComponante/>
        <p>Meu nome é {{ nome }}</p>
        <LifeCycle/>
        <Pessoa/>
    </div>
</template>

<script>
import Header from './components/Header.vue'
import PrimeiroComponante from './components/PrimeiroComponante.vue'
import LifeCycle from './components/LifeCycle.vue'
import Pessoa from  './components/Pessoa.vue'

export default({
    name: 'App',
    components: {
        PrimeiroComponante,
        Header,
        LifeCycle,
        Pessoa
    },
    data(){
        return {
            nome: 'Guilherme'
        }
    },
})
</script>

<style lang="scss" scoped>
    body{
        background-color: antiquewhite;
        div{
            background-color: aqua;
        }
    }
</style>
