<template>
    <div>
        <PrimeiroComponante/>
        <p>Meu nome é {{ nome }}</p>
        <LifeCycle/>
    </div>
</template>

<script>
import PrimeiroComponante from './components/PrimeiroComponante.vue'
import LifeCycle from './components/LifeCycle.vue'

export default({
    name: 'App',
    components: {
        PrimeiroComponante,
        LifeCycle
    },
    data(){
        return {
            nome: 'Guilherme'
        }
    },
    created(){
        this.nome = 'Gui'
    },
    mounted() {
        this.nome = 'Pedro'
    },
})
</script>
