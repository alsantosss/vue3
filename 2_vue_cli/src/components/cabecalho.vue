<template>

    <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">Serviços</a></li>
        <li><a href="#">Contato</a></li>
    </ul>

</template>

<script>
export default {
    name: "cabecalho"
}
</script>

<style scoped>
ul{
    list-style: none;
    display: flex;
    background: #111;
}
li{
    margin-right: 10px;
}
a{
    color: #ddd;
    text-decoration: none;
    transition: .5s;
}
a:hover{
    color: turquoise;
}
</style>