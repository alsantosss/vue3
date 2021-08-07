<template>
  <div>
    <primeiroComponente/>
    <p>Seguem os dados da aplicação --> {{dados}}</p>
    <lifeCyrcle />
    <pessoa />
  </div>
</template>

<script>
import primeiroComponente from './components/primeiroComponente.vue'
import lifeCyrcle from './components/lifeCyrcle.vue'
import Pessoa from './components/pessoa.vue'

  export default{
    name: 'App',
    components: {
      primeiroComponente,
      lifeCyrcle,
      Pessoa
    },
    data(){
      return {
        dados:"Exemplo"
      }
    },
    created(){
    setTimeout(() => {
          this.dados="Outra Coisa"
    }, 1000);
      
    },
    mounted(){
    setTimeout(() => {
          this.dados="Isso é Absurdo"
    }, 2000);
      
    }
  }
</script>
