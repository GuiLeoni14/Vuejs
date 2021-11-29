<template>
    <div>
        <h1>Olá vue</h1>
        <MultiplosEventos/>
    </div>
</template>

<script>
import MultiplosEventos from './MultiplosEventos.vue'

export default {
    name: 'PrimeiroComponante',
    components: {
        MultiplosEventos,
    }
}
</script>
