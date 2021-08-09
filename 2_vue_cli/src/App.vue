<template>
  <div>
    <cabecalho />
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
import cabecalho from './components/cabecalho.vue'

  export default{
    name: 'App',
    components: {
      cabecalho,
      primeiroComponente,
      lifeCyrcle,
      Pessoa
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
      this.lifeCyrcle()
    },
    methods:{
      lifeCyrcle(){
        console.log("Executou");
      }
    }
  }
</script>
<style>
body{
  background: #333;
  color: aliceblue;
}
a{
  color:aliceblue;
  text-decoration: none;
}
a:hover{
  color: green;
  text-decoration: none;
}
.bgemail{
  background: rgb(70, 105, 172);
}
</style>
