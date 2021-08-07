<template>
    <div>
        <p v-if="trabalhando">Estou trabalhando no momento.</p>
        <p v-else>Estou em busca de novas oportunidades.</p>
        <p>Utilizo as seguintes Tecnologias</p>
        <ul>
            <li>PHP</li>
            <li>Javascript</li>
            <li>Mysql</li>
            <li>HTML</li>
            <li>CSS</li>
        </ul>
        <p v-if="2>1">Dois é maior que um</p>
        <p v-show="email">Email: alsantosss@gmail.com</p>
        <p>Portfólio: <a v-bind:href="meu_link" target="_blank">Clique para ver o portfólio</a> </p>
        <avatar />
    </div>
</template>

<script>
import avatar from './avatar.vue'
export default {
  components: { avatar },
    nome: "info",
    data(){
        return {
            trabalhando: false,
            email:true,
            meu_link: "https://google.com.br"
        }
    } 
}
</script>