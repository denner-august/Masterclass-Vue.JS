<template>
  <div class="componente">
    <h1>componente with props</h1>
    <p>item: {{ item }}</p>
    <p>preço {{ preco }}</p>
  </div>
</template>

<script setup>
import { defineProps } from "vue";

defineProps({
  item: String,
  preco: Number,
});
</script>
