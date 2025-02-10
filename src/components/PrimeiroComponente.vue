<template>
<div>
    <h1>Olá vue fofinho</h1>
    <p>Meu nome é {{ nome }} e sou um {{ profissao }}</p>
</div>
</template>


<script>
    export default {
        name: 'PrimeiroComponente',
        data(){
            return{
                nome: "Matheus",
                profissao: "Dev"
            }
        }
    }
</script>
