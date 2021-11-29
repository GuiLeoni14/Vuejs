<template>
    <div>
        <Reutilizacao/>
        <h1>Olá vue</h1>
        <MultiplosEventos/>
        <Reutilizacao/>
        <Reutilizacao/>
        <Reutilizacao/>
        <Reutilizacao/>
    </div>
</template>

<script>
import MultiplosEventos from './MultiplosEventos.vue'
import Reutilizacao from './Reutilizacao.vue'

export default {
    name: 'PrimeiroComponante',
    components: {
        MultiplosEventos,
        Reutilizacao,
    }
}
</script>
