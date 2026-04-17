<script setup>
import { ref } from 'vue';

const frutas = ref(["Banana", "Uva", "Morango"])
const adicionarFruta = ref("")

function Adicionar() {
    if (adicionarFruta.value.trim() !== "") {
    frutas.value.push(adicionarFruta.value)
    adicionarFruta.value=""   
    }

}

</script>

<template>
<h2>Exercício 4</h2>

<form @submit.prevent="Adicionar">
    <input v-model="adicionarFruta" type="text" placeholder="Digite aqui..." required>
    <button>Adicionar</button>
</form>

<ul v-for="fruta in frutas" :key="fruta">
    <li>{{ fruta }}</li>
</ul>



<hr>

</template>