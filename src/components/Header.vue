<template>
    <header>
        <div class="container">
            <nav>
                <ul>
                    <li>teste</li>
                    <li>teste 2</li>
                </ul>
            </nav>
        </div>
    </header>
</template>
<script>
export default {
    name: 'Header',
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