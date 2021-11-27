<template>
    <div>
        <h2>Essa é a descriçãp da pessoa: {{ nome }}</h2>
        <Info/>
    </div>
</template>
<script>
import Info from './Info.vue'
export default {
    name: 'Pessoa',
    components: {
        Info
    },
    data (){
        return{
            nome: 'Guilherme'
        }
    }
}
</script>