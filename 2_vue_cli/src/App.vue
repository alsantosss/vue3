<template>
  <div>
    <primeiroComponente/>
    <p>Seguem os dados da aplicação --> {{dados}}</p>
  </div>
</template>

<script>
import primeiroComponente from './components/primeiroComponente.vue'
  export default{
    name: 'App',
    components: {
      primeiroComponente
    },
    data(){
      return {
        dados:"Exemplo"
      }
    }
  }
</script>
