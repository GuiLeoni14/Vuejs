<template>
    <div>
        <h2>Meu formulário: </h2>
        <form action="" @submit="enviarFormulario($event)">
            <div>
                <label for="nome">Nome:</label>
                <input type="text" name="nome" v-model="name" id="nome" placeholder="nome:">
            </div>
            <div>
                <label for="senha">senha:</label>
                <input type="text" name="senha" v-model="senha" id="senha" placeholder="senha:">
            </div>
            <div>
                <button type="submit">enviar formulario</button>
            </div>
        </form>
    </div>
</template>
<script>
export default {
    name: 'Form',
    data(){
        return{
            name: '',
            senha: '',
        }
    },
    methods: {
        enviarFormulario(e){
            e.preventDefault();
            const name = this.name;
            const senha = this.senha;
            console.log('Formulario enviado')
            console.log('O nome é: ' + name + 'A senha é: ' + senha);

            // Ajax
        }
    },
}
</script>