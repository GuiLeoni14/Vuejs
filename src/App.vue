<template>
    <div>
        <PrimeiroComponante/>
        <p>Meu nome é {{ nome }}</p>
        <LifeCycle/>
        <Pessoa/>
    </div>
</template>

<script>
import PrimeiroComponante from './components/PrimeiroComponante.vue'
import LifeCycle from './components/LifeCycle.vue'
import Pessoa from  './components/Pessoa.vue'

export default({
    name: 'App',
    components: {
        PrimeiroComponante,
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
