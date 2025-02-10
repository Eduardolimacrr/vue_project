<template>
    <div>
    <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
    <p v-else>Estou em busca de novas oportunidades!!</p>
    <p>Utilizo as seguintes tecnologias: </p>
    <ul>
        <li>JS</li>
        <li>Python</li>
        <li>vue</li>
    </ul>
    <p v-show="mostrar_email">Mande uma mensagem para: {{ email }}</p>
    <p>Para acessar meu portifólio basta clicar aqui <a v-bind:href="meu_link" target="blank">Basta clicar aqui</a></p>
    <Picture />
    </div>
</template>


<script>
import Picture from './Picture.vue'

    export default{
        name: 'Info',
        components: {
            Picture
        },
        data() {
            return{
                esta_trabalhando: true,
                mostrar_email: true,
                email: 'eduardolimacrr@gmail.com',
                meu_link: 'https://google.com'
            }
        }
    }
</script>
