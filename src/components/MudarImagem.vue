<template>
    <div>
        <button @click="$emit('mudarImagem')">Trocar de imagem </button>
    </div>
</template>

<script>
export default{
    name: 'MudarImagem',
    emits: ['mudarImagem']
}
</script>
