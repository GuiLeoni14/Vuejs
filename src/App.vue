<template>
    <div>
        <Header/>
        <PrimeiroComponante/>
        <p>Meu nome é {{ nome }}</p>
        <LifeCycle/>
        <Form/>
    </div>
</template>

<script>
import Header from './components/Header.vue'
import PrimeiroComponante from './components/PrimeiroComponante.vue'
import LifeCycle from './components/LifeCycle.vue'
import Pessoa from  './components/Pessoa.vue'
import Form from './components/Form.vue'

export default({
    name: 'App',
    components: {
        PrimeiroComponante,
        Header,
        LifeCycle,
        Pessoa,
        Form
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
