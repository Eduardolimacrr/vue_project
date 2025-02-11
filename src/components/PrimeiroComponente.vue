<template>
<div>
    <h1>Olá vue fofinho</h1>
    <p>Meu nome é {{ nome }} e sou um {{ profissao }}</p>
    <MultiplosEventos />
    <Reutilizacao />
</div>
</template>


<script>
    import MultiplosEventos from './MultiplosEventos.vue';
    import Reutilizacao from './Reutilizacao.vue';


    export default {
        name: 'PrimeiroComponente',
        components: {
            MultiplosEventos,
            Reutilizacao
        },
        data(){
            return{
                nome: "Matheus",
                profissao: "Dev"
            }
        }
    }
</script>
