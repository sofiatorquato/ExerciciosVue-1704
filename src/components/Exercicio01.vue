<script setup >
import { ref } from 'vue';


const contador = ref(0)

function Decrement() {
    contador.value--
}

function Increment() {
    contador.value++
}

</script>

<template>
<h2>Exercício 1</h2>
<h4> Contador: {{ contador }}</h4>
<button @click="Decrement">Diminuir</button>
<button @click="Increment">Aumentar</button>


</template>