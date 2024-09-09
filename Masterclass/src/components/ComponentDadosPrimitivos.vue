<template>
  <div class="componente">
    <h1>Component with date Reativos primitivos</h1>
    <p>Nome: {{ nome }} / Idade: {{ idade }}</p>
    <button v-on:click="fazerAniversario()">Fazer aniversário</button>
    <button @click="mudarNome()">Mudar nome</button>
  </div>
</template>

<script setup>
import { ref } from "vue";

const nome = ref("Denner");
const idade = ref(24);

function fazerAniversario(params) {
  idade.value++;
}

function mudarNome() {
  nome.value = "Mayara";
}
</script>
