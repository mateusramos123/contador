<script setup>
import { ref } from "vue"

const contador = ref(0)

function incrementar() {
  contador.value++
}

function decrementar() {
  contador.value--
}
</script>

<template>
  <h1>Contador do Mateus e Renan</h1>
  <p>Valor do Contador: {{ contador }}</p>
  <button v-on:click="incrementar">+</button>
  <button @click="decrementar">-</button>
</template>

<style scoped>
button {
  background-color: cadetblue;
  color: white;
  cursor: pointer;
  font-size: 16px;
  margin: 5px;
}
</style>
