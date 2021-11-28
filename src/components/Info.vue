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
    </div>
</template>
<script>
export default {
    name: 'Info',
    data() {
        return {
            esta_trabalhando: true,
            mostrar_email: true,
            email: 'teste@gmail.com'
        }
    },
}
</script>