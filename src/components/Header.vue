<template>
    <header>
        <div class="container">
            <nav>
                <ul>
                    <li>teste</li>
                    <li>teste 2</li>
                    <li v-if="esta_logado">Meu perfil</li>
                </ul>
            </nav>
        </div>
    </header>
</template>
<script>
export default {
    name: 'Header',
    props: ['esta_logado']
}
</script>

<style lang="scss" scoped>
    header{
        background-color: #ccc;
        .container{
            width: 100%;
            max-width: 100rem;
            nav{
                ul{
                    display: flex;
                    align-items: center;
                    justify-content: space-between;
                }
            }
        }
    }
</style>