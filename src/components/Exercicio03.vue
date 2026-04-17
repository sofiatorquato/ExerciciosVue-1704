<script setup>
import { ref } from 'vue';

const visivel = ref(true)

function Interuptor() {
    visivel.value=!visivel.value
}

</script>

<template>
    <h2>Exercicio 3</h2>
    <h1 v-if="visivel">Oi</h1>
    <button @click="Interuptor">{{visivel? "Esconder": "Mostrar"}}</button>
    <br>
    <hr>
</template>