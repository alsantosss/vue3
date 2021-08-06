<template>
    <div>
        <h1>Meu nome é: {{nome2}}</h1>
    </div>
</template>

<script>
export default{
    name: 'lifeCyrcle',
    data(){
        return {
            nome2: 'ainda não sei'
        }
    },
      created(){
        this.nome2 = "Jose"
    }
}
</script>
