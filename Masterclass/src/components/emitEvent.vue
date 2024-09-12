<template>
  <div class="componente">
    <h1>component emit event</h1>
    <p>{{ item }} (R$ {{ preco.toFixed(2) }})</p>
    <button @click="adicionar">adicionar ao carrinho</button>
  </div>
</template>

<script setup>
import { defineProps, defineEmits } from "vue";

const props = defineProps({
  item: String,
  preco: Number,
});

const emit = defineEmits(["foiAdicionado"]);

function adicionar() {
  emit("foiAdicionado", props.preco);
}
</script>

<style scoped>
.componente {
  width: 100%;
}
button {
  cursor: pointer;
  &:active {
    background-color: rgb(26, 99, 194);
  }
}
</style>
