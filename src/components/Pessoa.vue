<template>
    <div>
        <h2>Essa é a descriçãp da pessoa: {{ nome }}</h2>
        <Info :email="email" :esta_trabalhando=false />
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
            nome: 'Guilherme',
            email: 'email@dodata'
        }
    }
}
</script>