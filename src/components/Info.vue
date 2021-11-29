<template>
    <div>
        <p>{{ compEmail }} - {{ email }}</p>
        <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
        <p v-else>Utilizo as seguintes tecnologias:</p>
        <ul>
            <li v-for="(tecnologias, index) in backend_tecnologias" :key="index">{{ tecnologias }}</li>
        </ul>
        <p>Utiizo essas para frontend: </p>
        <ul>
            <li v-for="(tecnologias) in frontend_tecnologias" :key="tecnologias.id">
                {{ tecnologias.language }}
            </li>
        </ul>
        <div>
            <button @click="showEmail">Mostrar email</button>
        </div>
        <p v-show="mostrar_email">Mande seu email para: {{ email }}</p>
        <p>para acessar meu portfoilio basta <a v-bind:href="meu_link">clicar aqui</a></p>
        <Picture/>
    </div>
</template>
<script>
import Picture from "./Picture.vue"
export default {
    name: 'Info',
    components: {
        Picture,
    },
    props: {
        email: String,
        esta_trabalhando: Boolean,
    },
    data() {
        return {
            mostrar_email: false,
            meu_link: 'google.com',
            backend_tecnologias: ['JavaScript', 'PHP', 'Python'],
            frontend_tecnologias: [
                {id: 1, language: 'HTMl'},
                {id: 2, language: 'SCSS'},
                {id: 3, language: 'jAVASCRIPT'},

            ]
        }
    },
    methods: {
        showEmail(){
            this.mostrar_email = !this.mostrar_email
            console.log('Mostrando email')
        }
    },
}
</script>