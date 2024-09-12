<template>
  <div class="componente">
    <h1>componente com propriedades computadas</h1>
    <p>{{ idade }}</p>
    <label>ano nacimento:</label>
    <input type="number" v-model="anoAtual" min="1900" />
    <label>ano Atual:</label>
    <input type="number" v-model="anoNacimento" min="200" />
  </div>
</template>

<script setup>
import { ref, computed } from "vue";

const anoNacimento = ref(1900);
const anoAtual = ref(2000);
const idade = computed(() => {
  return anoNacimento.value - anoAtual.value;
});
</script>
