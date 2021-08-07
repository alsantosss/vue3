<template>
    <div>
        <h1>Esta é a descrição da Pessoa {{nome}}</h1>
        <info />
        <div><input-text /></div>
        <div><input-text /></div>
        <div><submit /></div>
    </div>
</template>

<script>
import InputText from './form/inputText.vue'
import Submit from './form/submit.vue'
import info from './info.vue'
export default{
  components: { info, InputText, Submit },
    nome: "Andre",
    data(){
        return {
            nome:"Andre"
        }
    }
}
</script>
