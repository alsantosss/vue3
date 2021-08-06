<template>
    <div>
        <h1>Olá Vue</h1>
    <p>Meu nome é {{nome}} e trabalho como {{profissao}}</p>
    </div>
</template>

<script>
export default {
    name: 'primeiroComponente',
    data(){
        return{
            nome:"Andre Santos",
            profissao:"programador"
        }
    }
}
</script>