<template>
<div>
    <h1>Meu nome é: {{ nome }} </h1>

</div>

</template>

<script>
    export default {
        name: 'LyfeCycle',
        data () {
            return{
                nome: 'Ainda n sei'
            }
        },
        created(){
            setTimeout(() => {
                this.nome = 'MAtheus'
            }, 1000);

            this.lifeCycle()
        },
        mounted(){
            setTimeout(() => {
                this.nome = 'Pedro'
            }, 2000);

            this.lifeCycle()
        },
        methods: {
            lifeCycle() {
                console.log("Executou");
            }
        }
    }
</script>
