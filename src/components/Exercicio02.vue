<script setup>
import { ref } from 'vue';

const message=ref("")


function LimparPesquisa() {
    message.value=""
}
</script>

<template>
    <hr>
    <h2>Exercício 2</h2>

<input v-model="message" type="text" placeholder="Digite aqui">
<h4>{{ message }}</h4>

<button @click="LimparPesquisa">Limpar</button>
<hr>
</template>