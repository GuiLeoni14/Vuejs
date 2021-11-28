<template>
    <div>
        <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
        <p v-else>Utilizo as seguintes tecnologias:</p>
        <ul>
            <li>Python</li>
            <li>JavaScript</li>
            <li>PHP</li>
        </ul>
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
    data() {
        return {
            esta_trabalhando: true,
            mostrar_email: true,
            meu_link: 'google.com',
            email: 'teste@gmail.com'
        }
    },
}
</script>