<script setup>
import { ref } from 'vue';

const ativo = ref(false)

function Interuptor() {
    ativo.value=!ativo.value
}

</script>

<template>
<h2>Exercico 5</h2>

<h4 :class="{'sucesso':ativo}">Texto</h4>
<button @click="Interuptor">
Clique
</button>

<hr>
</template>

<style scoped>

.sucesso{
    color: green;
}

</style>