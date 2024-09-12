<template>
  <div class="componente">
    <h1>Componente for listening event</h1>
    <p>total R$ {{ total }}</p>
    <div class="lista">
      <EmitEvent item="item1" :preco="1.99" @foi-adicionado="updatePrice" />
      <EmitEvent item="item2" :preco="5.0" @foi-adicionado="updatePrice" />
      <EmitEvent item="item3" :preco="1.99" @foi-adicionado="updatePrice" />
    </div>
  </div>
</template>

<script setup>
import EmitEvent from "./emitEvent.vue";
import { ref } from "vue";

const total = ref(0);

function updatePrice(t) {
  const valor = total.value + t;
  total.value = +valor.toFixed(2);
}
</script>

<style scoped>
.lista {
  display: flex;
  justify-content: space-between;
}
</style>
