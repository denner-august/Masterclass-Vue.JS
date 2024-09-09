<template>
  <div class="componente">
    <h1>Component with date Reativos não primitivos</h1>
    <p>Nome: {{ pessoa.nome }} / Idade: {{ pessoa.idade }}</p>
    <button @click="fazerAniversario()">Fazer aniversário</button>
    <button @click="mudarNome()">Mudar nome</button>
  </div>
</template>

<!--
  
<script setup>
import { reactive } from "vue";

const pessoa = reactive({ nome: "nunes", idade: 30 });

function fazerAniversario(params) {
  pessoa.idade++;
}

function mudarNome() {
  pessoa.nome = "Mayara";
}
</script>
-->

<script>
export default {
  data: function () {
    return {
      pessoa: {
        nome: "nunes",
        idade: 30,
      },
    };
  },

  methods: {
    fazerAniversario() {
      this.pessoa.idade++;
    },

    mudarNome() {
      this.pessoa.nome = "Mayara";
    },
  },
};
</script>
